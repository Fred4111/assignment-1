public class ClassAverage {

    // Version 1: Two scores
    public static double calculateClassAverage(double score1, double score2) {
        return (score1 + score2) / 2.0;
    }

    // Version 2: Three scores
    public static double calculateClassAverage(double score1, double score2, double score3) {
        return (score1 + score2 + score3) / 3.0;
    }

    // Version 3: Array of scores
    public static double calculateClassAverage(double[] scores) {
        double sum = 0.0;
        for (double s : scores) {
            sum += s;
        }
        return scores.length == 0 ? 0 : sum / scores.length;
    }

    // Testing the methods
    public static void main(String[] args) {
        System.out.println(calculateClassAverage(80, 90));                 // 2 scores
        System.out.println(calculateClassAverage(70, 85, 90));             // 3 scores
        System.out.println(calculateClassAverage(new double[]{60,75,80,95})); // array
    }
}
