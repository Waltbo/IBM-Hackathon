# Array-Rotation
Method to rotate an array to the left N number of times

    static int[] rotLeft(int[] a, int d) {
        int counter=0;
    
        int[] tempArray = new int[a.length];
        for(int i=0; i<a.length;i++){
            tempArray[i]=a[((counter++)+d%a.length];
        }
        return tempArray;
        
    }
# Sparse-Arrays

Method to see how many times a string appears in a query

    static int[] matchingStrings(String[] strings, String[] queries) {
        int[] timesPassed= new int[queries.length];
        for(int i=0;i<queries.length; i++){
            for(int j=0;j<strings.length;j++){
                if(strings[j].equals(queries[i])){
                    timesPassed[i]+=1;
                }
            }
        }
        return timesPassed;
    }
# Two-Strings

Method to check if strings contain similar characters

static String twoStrings(String s1, String s2) {
        String [] check = s1.split("");
        for(int i=0; i<check.length;i++){
            if(s2.contains(check[i])){
                return "YES";
            }
        }
        return "NO";
    }
