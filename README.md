# -Minimum-Number-of-Moves-to-Seat-Everyone
class Solution {
    public int minMovesToSeat(int[] seats, int[] students) {
        int d=0;
        Arrays.sort(seats);
        Arrays.sort(students);
        for(int i=0;i<seats.length;i++)
            {
               d+=Math.abs(seats[i]-students[i]);
            }return d;                                                                        
        
    }
}
output
