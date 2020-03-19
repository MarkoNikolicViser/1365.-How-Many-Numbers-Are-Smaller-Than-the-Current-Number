public class Solution {
    public int[] SmallerNumbersThanCurrent(int[] nums) {
             int brojac = 0;
          
       
            List<int> lista = new List<int>() { };
            foreach (var y in nums)
            {
                foreach (var x in nums)
                    if (y > x)
                        brojac++;


                lista.Add(brojac);
                brojac = 0;
            }
        int []str=lista.ToArray();
        return str;
    }
}
