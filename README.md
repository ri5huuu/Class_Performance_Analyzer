import java.util.Scanner;

public class classperformanceanalyzer {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int maximumMarks = 80;//maximum marks that can be scored.
        int markLimit = 50;//class avg limit to track progress.
        System.out.println("Maximum Marks is 80");
        char percentage = '%';

        System.out.println("Mark obtained by a: ");
        float marks_a = sc.nextFloat();
        if (marks_a > maximumMarks) {
            throw new IllegalArgumentException("DUMB ERROR");
        }
        float per = marks_a/maximumMarks * 100;
        System.out.println("Percentage: " + per + percentage );


        System.out.println("Mark obtained by b: ");
        float marks_b = sc.nextFloat();
        if (marks_b > maximumMarks){
           throw new IllegalArgumentException("DUMB ERROR");
        }
        float per_1 = marks_b/maximumMarks * 100;
        System.out.println("Percentage: " + per_1 + percentage);


        System.out.println("Mark obtained by c: ");
        float marks_c = sc.nextFloat();
        if (marks_c > maximumMarks) {
            throw new IllegalArgumentException("DUMB ERROR");
        }
        float per_2 = marks_c/maximumMarks * 100;
        System.out.println("Percentage: " + per_2 + percentage );


        System.out.println("Mark obtained by d: ");
        float marks_d = sc.nextFloat();
        if (marks_d > maximumMarks) {
            throw new IllegalArgumentException("DUMB ERROR");
        }
        float per_3 = marks_d/maximumMarks * 100;
        System.out.println("Percentage: " + per_3 + percentage);


        System.out.println("Average Marks: ");
        float meanMarks = (marks_a + marks_b + marks_c + marks_d) / 4;
        System.out.println(meanMarks);

        if (meanMarks > markLimit){
            System.out.println("Good progress!!!");
        }
        else{
            System.out.println("Improvement required!!!");
        }

    }
}
