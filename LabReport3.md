# **Lab Report 3**
***
## Part 1 - Bugs ArrayList ReverseInPlace
### 1. Fail-inducing Input
` @Test
  public void testReverseInPlace1() {  
    int[] input2 = {1, 2, 3, 4};  
    ArrayExamples.reverseInPlace(input2);  
    assertArrayEquals(new int[]{4,3,2,1}, input2);  
  } `  

  ### 2. Non-Fail-Inducing Input
` @Test  
	public void testReverseInPlace() {  
    int[] input1 = { 3 };  
    ArrayExamples.reverseInPlace(input1);  
    assertArrayEquals(new int[]{ 3 }, input1);  
	} `  

 ### 3. The Symptom
 //put image here

### 4. Debugging
**Before**
`static void reverseInPlace(int[] arr) {  
    for(int i = 0; i < arr. length; i += 1) {  
    arrlil = arrlarr.length - i - 11;  
 }`

**After**
`static void reverseInPlace(int[] arr) {  
    for(int i = 0; i < arr.length / 2; i += 1) {  
      int temp = arr[i];  
      arr[i] = arr[arr.length - i - 1];  
      arr[arr.length - i - 1] = temp;  
    }  
  }
  `
