# Left-Rotation
Method to rotate an array to the left N number of times

    static int[] rotLeft(int[] a, int d) {
        int counter=0;
    
        int[] tempArray = new int[a.length];
        for(int i=0; i<a.length;i++){
            tempArray[i]=a[((counter++)+d%a.length];
        }
        return tempArray;
        
    }
#Spare-Arrays

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
