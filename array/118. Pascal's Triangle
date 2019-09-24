class Solution {
    public List<List<Integer>> generate(int numRows) {
        List<List<Integer>> res = new ArrayList<>();
        if (numRows == 0) return res;
        List<Integer> tmp = new ArrayList<>();
        tmp.add(1);
        res.add(tmp);
        if (numRows == 1) return res;
        for (int i = 2; i <= numRows; i++) {
            tmp = new ArrayList<>();
            for (int j = 0; j < i; j++) {
                if (j == 0 || j == i-1) tmp.add(1);
                else tmp.add(res.get(i - 2).get(j - 1) + res.get(i - 2).get(j));
            }
            res.add(tmp);
        }
        return res;
        
    }
}
