# Decompress-Run-Length-Encoded-List
class Solution:
    def decompressRLElist(self, nums: List[int]) -> List[int]:
        n=len(nums)
        r=[]
        for i in range(0,n,2):
            f=nums[i]
            c=nums[i+1]
            for j in range(f):
                r.append(c)
        return r
