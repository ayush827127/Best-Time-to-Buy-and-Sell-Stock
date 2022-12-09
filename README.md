# Best-Time-to-Buy-and-Sell-Stock
find the maximum profit you can gain in the given array






	public int stock(int[] arr) {

		int arr[] = {7,6,4,3,1};
		int buy = arr[0];
		int sell = arr[0];
		
		for(int i = 0; i < arr.length - 1; i++) {
			if(buy > arr[i+1] ) {
				buy = arr[i+1];
				sell = arr[i+1];
			}
			else{
			if(sell < arr[i+1]){
			   sell = arr[i+1];
			}
			}
		}
		return (sell - buy);

	}


