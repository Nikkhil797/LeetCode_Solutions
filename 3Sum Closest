class Solution {
public:
    int threeSumClosest(vector<int>& arr, int t) {
        int n = arr.size();
        sort(arr.begin(), arr.end());
        int ans = INT_MIN;
        for(int first = 0;first<=n-3;first++){
            int sec = first+1, third = n-1;
			// Two sum technique for second and third element
            while(sec < third){
                int sumtemp = arr[first] + arr[sec] + arr[third];
                if(sumtemp == t){
                    return sumtemp;
                }
                if(sumtemp < t ){
                    if(ans == INT_MIN) ans = sumtemp;
                    else{
                        if(abs(ans-t) > abs(sumtemp-t)) ans = sumtemp;
                    }
                    sec++;
                }
                else{
                    third--;
                    if(ans == INT_MIN) ans = sumtemp;
                    else{
                        if(abs(ans-t) > abs(sumtemp-t)) ans = sumtemp;
                    }
                }
            }
            
        }
        return ans;
    }
};
