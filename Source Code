import edu.duke.*;

public class wordplay
{
   public String isvowel(char ch)
   { 
    
       if(ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o'  || ch == 'u' ||ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U')
       {
           
           return "true";
    
    
    
    }
    
    else 
    {
        return "false";
    
    }
    
    
}


public void testisVowel()
{
      String result = isvowel('a');
      System.out.println(result);
}    



public String replaceVowel(String input) {
    
    StringBuilder sb = new StringBuilder(input);
    
     for(int i = 0; i < sb.length(); i++)
      {
        char currchar = sb.charAt(i);
        
        if(isvowel(currchar) == "true" )
        {
             sb.setCharAt(i, '*');
        }
        
        
        }  return sb.toString();    

 

}

  public void testreplaceVowel()
  {
    String  character   = replaceVowel("hEllo world");
    System.out.println(character);
    }

    
public String emphasize(String input, char ch)
 {
    StringBuilder sdf = new StringBuilder(input);
    for(int i = 0;i<sdf.length();i++)
    {
    
        char currchar = sdf.charAt(i);
        if(currchar == ch)
           
           {
             if((i/2) == 0)
             {
                sdf.setCharAt(i, '*');
                }
                
              else 
             {   sdf.setCharAt(i, '+');
            }
            
            
            
          
    }
    
    
    
}     return sdf.toString();
          
        }

        
        public void testemphasize()
        {
             String result = emphasize("lock him up", 'o');
             System.out.print(result);
        
        
        
        }
        
        
        
    
    public String encrypt(String input, int key) {
        //Make a StringBuilder with message (encrypted)
        StringBuilder encrypted = new StringBuilder(input);
        //Write down the alphabet
        String alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
        //Compute the shifted alphabet
        String shiftedAlphabet = alphabet.substring(key)+
        alphabet.substring(0,key);
        //Count from 0 to < length of encrypted, (call it i)
        for(int i = 0; i < encrypted.length(); i++) {
            //Look at the ith character of encrypted (call it currChar)
            char currChar = encrypted.charAt(i);
            if(Character.isUpperCase(currChar))
            {
            //Find the index of currChar in the alphabet (call it idx)
            int idx = alphabet.indexOf(currChar);
            //If currChar is in the alphabet
            if(idx != -1){
                //Get the idxth character of shiftedAlphabet (newChar)
                char newChar = shiftedAlphabet.charAt(idx);
                //Replace the ith character of encrypted with newChar
                encrypted.setCharAt(i, newChar);
            }
            //Otherwise: do nothing
        }
        //Your answer is the String inside of encrypted
        else
        {      int idx = alphabet.toLowerCase().indexOf(currChar);
             
            if(idx != -1)
            {
                 char newChar = shiftedAlphabet.toLowerCase().charAt(idx);
                 encrypted.setCharAt(i, newChar);
            
            }
            
        
        
        
        }
        
    } 
        return encrypted.toString();
    }
    public void testCaesar() {
        int key = 17;
        FileResource fr = new FileResource();
        String message = fr.asString();
        String encrypted = encrypt(message, key);
        System.out.println(encrypted);
        String decrypted = encrypt(encrypted, 26-key);
        System.out.println(decrypted);
    }
        
    
    public String encrypttwokeys(String input,int key1,int key2)
    {
       
     StringBuilder encrypted = new StringBuilder(input);
       //Write down the alphabet
        String alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
        //Compute the shifted alphabet
        String shiftedAlphabet1 = alphabet.substring(key1)+
        alphabet.substring(0,key1);
        String shiftedAlphabet2 = alphabet.substring(key2) + alphabet.substring(0,key2);
        //Count from 0 to < length of encrypted, (call it i)
        for(int i = 0; i < encrypted.length(); i++) 
        
        {
            //Look at the ith character of encrypted (call it currChar)
            char currChar = encrypted.charAt(i);
            if((i%2) == 0)
            {
            if(Character.isUpperCase(currChar))
            {
            //Find the index of currChar in the alphabet (call it idx)
            int idx = alphabet.indexOf(currChar);
            //If currChar is in the alphabet
            if(idx != -1){
                //Get the idxth character of shiftedAlphabet (newChar)
                char newChar = shiftedAlphabet1.charAt(idx);
                //Replace the ith character of encrypted with newChar
                encrypted.setCharAt(i, newChar);
            }
            //Otherwise: do nothing
        }
        //Your answer is the String inside of encrypted
        else
        {      int idx = alphabet.toLowerCase().indexOf(currChar);
             
            if(idx != -1)
            {
                 char newChar = shiftedAlphabet1.toLowerCase().charAt(idx);
                 encrypted.setCharAt(i, newChar);
            
            }
            
        }
        
        
        }
        
       if((i%2) == 1)
        
        
          {
            if(Character.isUpperCase(currChar))
            {
            //Find the index of currChar in the alphabet (call it idx)
            int idx = alphabet.indexOf(currChar);
            //If currChar is in the alphabet
            if(idx != -1){
                //Get the idxth character of shiftedAlphabet (newChar)
                char newChar = shiftedAlphabet2.charAt(idx);
                //Replace the ith character of encrypted with newChar
                encrypted.setCharAt(i, newChar);
            }
            //Otherwise: do nothing
        }
        //Your answer is the String inside of encrypted
        else
        {    
            int idx = alphabet.toLowerCase().indexOf(currChar);
             
            if(idx != -1)
            {
                 char newChar = shiftedAlphabet2.toLowerCase().charAt(idx);
                 encrypted.setCharAt(i, newChar);
            
            }
            
        }
    }
        
        } 
        
        
        
        
        
        
     
        return encrypted.toString();
    }
    public void testencrypttwokeys() {
        int key1 = 23;
        int key2 = 17;
       
        String encrypted = encrypttwokeys("First legion", key1, key2);
        System.out.println(encrypted);
        
    }
    
    
    
    
    }
    
         
 
 
