Function Calling LLMs
General Purpose LLMs
	Respond to all types of queries
	Including function calling
		OpenAI GPT-x
		Gemini
		Mistral
		Etc
		
Special Purpose LLMs
	Highly trained to focus on a single or small set of tasks
		Raven-13B
			Tuned to provide function calling services
			Will always try to return a function
			Smaller and lower latency than general purpose LLMs
			
Function Calling, Tools?
"Function Calling": is the name given to this LLM capability of forming a string containing a function call or structure needed to make a function call.
"Tools" are the functions being called 

With Function calling
The LLM is trained to understand the function description passed in prompt, it can return the string to invoke the function eg.
i\p to LLM
User query -> "What is the temperature in New York?
Function Des -> getTemp(city_name:string)

o\p from LLM  getTemp(city_name="New York")

They only generate the string to call functions and do not actually make the call.

