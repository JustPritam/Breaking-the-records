# Breaking-the-records
{
    ArrayList<Integer> res=new ArrayList<Integer>();
    int min=scores.get(0);
    int max=scores.get(0);
    int m=0;int x=0;
    for(int i=0;i<scores.size();i++)
    {
        if(scores.get(i)<min)
        {
            min=scores.get(i);
            m++;
        }
        else if(scores.get(i)>max)
        {
            max=scores.get(i);
            x++;
        }
    }
    res.add(x);
    res.add(m);
    return res;
}
