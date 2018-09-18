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
