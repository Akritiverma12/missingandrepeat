# missingandrepeat
 vector<int> findTwoElement(vector<int>& arr) {
        int n=arr.size();
        int m=n+1;
        int hash[m]={0};
        for(int i=0;i<n;i++){
            hash[arr[i]]++;
        }
        int re=-1;
        int mi=-1;
        for(int i=1;i<m;i++){
            if(hash[i]==2)re=i;
            if(hash[i]==0)mi=i;
        }
        vector<int>ans;
        ans.push_back(re);
        ans.push_back(mi);
        return ans;
        
    }
