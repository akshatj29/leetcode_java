class Solution {
    public String longestPalindrome(String s) {
        
        if(s.length()<2)
            return s;
        String currMaxSubs = s.substring(0,1);
        
        for(int i=0;i<s.length();i++)
        {
            for(int j=i+1;j<=s.length();j++)
            {
                if(isPalindrome(s.substring(i,j)) && s.substring(i,j).length() > currMaxSubs.length())
                    currMaxSubs = s.substring(i,j);
            }
        }
        
        return currMaxSubs;
    }
    
    public boolean isPalindrome(String s) 
    {
        StringBuilder sb = new StringBuilder(s);
        if((sb.reverse().toString()).equals(s))
            return true;
        else
            return false;
    }
}
