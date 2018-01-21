package ScherbunaV;


import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.util.ArrayList;
import java.util.Arrays;
import java.util.List;

public class Sort {
    public static void main(String[] args) throws IOException{
        BufferedReader r = new BufferedReader(new InputStreamReader(System.in));
        String sents = r.readLine();
        String[] arr = sents.split(" ");
        List<String> list = Arrays.asList(arr);
        ArrayList<String > newlist = new ArrayList<>();
        newlist.addAll(list);

        for(int i = 0; i < newlist.size();){
            if(newlist.get(i).length()%2 != 0)
                newlist.remove(i);
            else
                i++;
        }
        
        int n = newlist.get(0).length();
        int index = 0;
        for(int i = 1; i < newlist.size(); i++){
            if(n < newlist.get(i).length()) {
                n = newlist.get(i).length();
                index = i;
            }
        }
        System.out.println(newlist.get(index));
    }
}
