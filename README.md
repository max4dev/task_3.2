# task_3.2

public class Main {

    public static void main(String[] args) {

        int numbers[][] = {
                {1,   2,  3,  4},
                {-1, -2, -3, -4},
                {3,   5,  3,  1},
                {5,   5, 10,  4},
        };
        for (int i = 0; i < 4; i++) {
            int minimum = min(numbers [i][0], numbers [i][1], numbers [i][2], numbers [i][3]);
                System.out.println("Минимальное значение в строке " + (i+1) + " : " + minimum);
        }
    }

    static int min (int a, int b, int c, int d) {
        if (min(a, b) > min(c, d)) return min(c, d);
        else return min(a, b);
    }

    static int min (int a, int b) {
        if (a>b) return b;
        else return a;
    }
}
