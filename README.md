1. What was the most confusing thing in this lab? Be specific.

The most confusing part for me was understanding how matrix dimensions work during the dot product operations in Exercise 7. Visualizing what happens when a (5, 4) matrix is multiplied by a (4,) vector took me some time to grasp. Also, grasping the concept of "broadcasting" in NumPy, like when we subtracted the mean from the entire feature matrix at once during manual data scaling, felt a bit unintuitive at first. However, printing out the shapes (.shape) at each step really helped me figure it out.

2. What does the dot product in section 3.6 have to do with a neuron? Explain it in your own words. 

A biological neuron receives multiple signals, gives different importance to each signal, and then sums them up to decide whether to activate or not. In our code, the dot product does exactly this mathematical process: it multiplies every single incoming feature (input) by its corresponding importance measure (weight) and adds all of these products together into a single number. So basically, computing a dot product is just an efficient, mathematical way of calculating a neuron's total incoming stimulation before passing it to an activation function like the sigmoid.

3. Why do we split data into training and test sets? What could go wrong if we didn't? 

We split the data because we need a way to prove that our neural network has actually learned the underlying patterns rather than just memorizing the examples we showed it. The test set acts as an "unseen final exam" to evaluate the model's true, real-world performance. If we evaluated the model using the exact same data it trained on, it would be like giving a student the answer key before a test; it would score 100% easily but fail miserably when faced with a slightly different, new problem (a problem known as "overfitting").
