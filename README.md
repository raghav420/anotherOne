# anotherOne
package com.companie;

public class SortArray {
    public static void main(String[] args) {
       System.out.println(contains(ar,0,30));
    }

   static int[] ar={10,20,30,40,50,60};
    public static int findFirst(int[] array,int index,int item ) {
        if (index == array.length) {
            return -1;
        }
        if (array[index] == item) {
            return index;
        } else {
            return findFirst(array, index + 1, item);
        }


    }
public static boolean contains(int[] nums,int index,int item) {
    if (index == nums.length) {
        return false;
    }
    return nums[index] == item || contains(nums, index + 1, item);
}







}
