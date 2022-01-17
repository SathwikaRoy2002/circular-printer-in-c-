# circular-printer-in-c++(logic)
long getTime(string s) {
    int count=0;
    count+=min(abs(s[0]-'A'),25-abs(s[0]-'A')+1);
    for(int i=0;i<s.length()-1;i++)
    { 
             count+=min(abs(s[i]-s[i+1]),25-abs(s[i]-s[i+1])+1);
    }
    return (long)count;

}
