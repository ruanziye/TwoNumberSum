# TwoNumberSum
作业
public class TwoNumberSum {
    public static void main(String[] args) {
        //给定数组数据
        int[] arr={1,3,5,7,9,11};
        //输入target
        System.out.println("请输入目标值（target）：");
        //获取输入target
        int target = new Scanner(System.in).nextInt();
        //调用方法计算，返回结果数组
        //int[] arr2=calculate(arr,target);
        int[] arr2=solution(arr,target);
        //进行判断
        while (arr2 == null){
            System.out.println("数组中没有可以合成该target的两个数！请输入其他target：");
            target = new Scanner(System.in).nextInt();
            arr2=calculate(arr,target);
        }
        //输出
        System.out.println("合成该target数组下标为："+ Arrays.toString(arr2));


    }
