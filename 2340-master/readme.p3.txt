Nina Moorman
nmoorman3@gatech.edu

private String calc(String input) {
		//Person 3 put your implementation here

		// dont change inout, copy
		String copy = input;
		String out = "";

		// go through input
		for (int i = 0; copy.length() > 0; i++){

			// save last letter
			char saved = copy.charAt(copy.length() -1);

			// add to end of new word
				// cat --> t --> ta --> tac
			out = out + saved;

			// delete that char of the input
			if (copy.length() == 1) {
				copy = "";
			} else {
				copy = copy.substring(0, copy.length() - 1);
			}
		}
		return out;
	}