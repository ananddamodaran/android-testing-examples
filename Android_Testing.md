Testing
 - test the feature what is intended
 - UI testing 
 - Espresso
     * Steps to Manually UI Test
         1. Find the view
		onView(ViewMatcher)
	 2. Perform action on the view
		.perform(ViewAction)
  	 3. Check if the view does what you expected
		Assertion - A check to see if what we expected matches what actually happened
		ViewAssertion - A class with methods that help us perfom assertions, or checks on Views
      		.perform(ViewAssertion) 
     * Tests intents with Espresso
 	 1. Intent Testing
	      - A small piece of code that acts as a fake response to an intent call during a test
	      - The benefit of using a stub is that it gives us consistent results and allows us to focus on action at a time
	      - For testing intent responses
	      - intending(Matcher(Intent> matcher)
	 2. Intent Verification
	      - Using a hardcoded matcher to verify that the information we intended to send in an intent is what was actually sent
	      - intended(Matcher<Intent> matcher, VerificationMode verification
      * Espresso waits until the app is idle, or not doing anything, to perform the next action
	  When is an app idle?
             - No UI events in the current message queue
	     * No more tasks in the default AsnynTask thread pool
    
