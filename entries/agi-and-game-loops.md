<h1 align="center">Artificial General Intelligence and Game Loops</h1>

_Written September 2nd, 2020._

---

I'm going to be honest. I have no idea what the direction of artificial general intelligence is taking. It seems like we constantly try to treat AI, (namely machine learning learning branches) as simple input-output machines. Our minds don't work like that. We're continously moving, thinking, processing entities. There's no such thing as idling or waiting for input for us. Yes, I know that reinforcement learning algorithms are much closer to acting as a continously moving machine but I feel it's not quite there, yet.

I believe that if there is a future in artificial general intelligence, we should be looking into algorithms that act more like game loops rather than trainable functions. A continously running service; something that processes and analyzes itself even if nothing has changed. A model that is constantly training and learning, even after deployed. I believe this is possible. It's all about finding a comfortable medium.

My initial goal for tackling this problem was to describe a platform that would be trainable, yet domain agnostic. It would have to be something that could be continously running and processing data as it sees fit. It needs to handle passing instructions to other parts of the agent without needing to worry about how those elements are proccessed. It should be able to query for information at will, regardless if that information is coming from sensory input, a database, memory reserves, etc. Lastly, it needs to be able to recive important information and react to that information in any way that it desires. To me, this sounds a lot like an SSH terminal, doesn't it? The agent doesn't need to worry about how each command works or how it's implemented. Really, the AI just needs to learn how to write commands and pipe them into each other. It doesn't really need to worry about what the commands are or anything. Just when to use them. Information can be continously feed into the agent as data is recieved. Command outputs and such as well.

In this situation, the visible state is simply what the AI can currently see in the console, while the nonvisible state must be queried by the agent constantly. It's also worth noting that, while this approach can be done in text, using language is not needed. Tasks such as NLP would be done by the commands, not the core agent process. In the end, the agent only needs to learn 3 things:

1) How to write a command.
2) How to make commands interact.
3) How to process the current state.

Commands are not promised to return the same output for the same inputs, as they closely interact with the real environment. As such, the agent needs to be learn how to react with different outputs, regardless of what they are. Since the agent is continously learning, even after deployment, in theory, it should keep adapting to the world as it changes.

Additional notes:

I would also think that it would be quite easy to keep building onto the agent by adding more and more commands, thus extending it's capabilities. Right? My only question would be able how to make the agent resize itself as it learns. There's only so much space in a neural network. That'll eventually fill up as it gets a better understanding of the world. What happens when it's full?
