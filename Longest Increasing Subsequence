package dp;
import java.util.*;
class Solution {
  public int LongestIncreasingSubsequence(int[] arr) {
    int n = arr.length;
    int[] dp = new int[n];

    int res = 0;

    for (int i = 0; i < n; i++) {

      Integer max = null;

      for (int j = 0; j < i; j++) {

        if (arr[j] < arr[i]) {

          if (max == null || dp[j] > max) {

            max = dp[j];
          }
        }
      }

      if (max != null) {

        dp[i] = max + 1;

      } else {
        dp[i] = 1;
      }

      if (dp[i] > res) {
        res = dp[i];
      }
    }

    return res;
  }
}
