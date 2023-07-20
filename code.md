public class ss {
    public static void array(int arr[]){
        int lar[]=new int[arr.length];
        int k=0;
        int max;
        int last=arr[arr.length-1];
       for(int i=0;i< arr.length;i++){
            max=arr[i];
           for(int j=i+1;j<arr.length;j++){
               if(max<arr[j]){
                   break;
               }
               else{
                   lar[k]=max;
               }
           }
           k++;
       }
       int sum=0;
        for(int i=0;i< lar.length;i++){
           sum=sum+lar[i];
        }
        int res=sum+last;
        System.out.println(res);
    }
    public static void main(String[] args) {
        int arr2[]={52,66,64,36,45,24,32};
        array(arr2);
    }

}
