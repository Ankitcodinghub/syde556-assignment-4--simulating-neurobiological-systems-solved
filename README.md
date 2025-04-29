# syde556-assignment-4--simulating-neurobiological-systems-solved
**TO GET THIS SOLUTION VISIT:** [SYDE556 Assignment 4- Simulating Neurobiological Systems Solved](https://www.ankitcodinghub.com/product/syde556-solved-2/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;110312&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;SYDE556 Assignment 4- Simulating Neurobiological Systems  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Important Notes – Please Read Carefully

• Please use Python 3 along with the numpy and matplotlib libraries to solve these assignments.

In particular, fill out this Jupyter Notebook template:

https://github.com/astoeckel/syde556-w20/blob/master/assignments/assignment_04/ syde556_assignment_04_template.ipynb

• Clearly label any plot you produce, including the axes. Provide a legend if there are multiple graphs in the same plot.

• You won’t be judged on the quality of your code, but writing reusable functions will greatly simplify this and future assignments.

• For this assignment, you must use Nengo. Feel free to look through the examples folder and/or the tutorials on the Nengo website before doing this assignment.

1 Building an ensemble of neurons

Make a new model with a single ensemble of neurons. It should have 100 neurons, and represent a 1dimensional space. The intercepts should be between −1 and 1, and the maximum firing rates should be between 100Hz and 200Hz. τRC should be 20ms and τref should be 2ms.

🖈 You don’t need to run the model over time for this question.

[0.5] a) Tuning curves. Plot the population tuning curves. Plot the representation accuracy plot (x − xˆ).

Compute and report the RMSE.

🐍 Feel free to have a look at this Nengo tutorial to solve this question.

🐍 Create a “dummy” identity connection from the ensemble to itself to have Nengo compute the population identity decoders. Then, you can use nengo.utils.connection.eval_point_decoding to compute xˆ. Nengo will take care of computing the decoders under noise. You don’t have to use your code from previous assignments, but, of course, feel free to do so. In this case, compute the decoders under the assumption of noise with a magnitude of σ = 0.1 · 200Hz.

[0.5] b) RMSE and radius. Compute the RMSE for (at least) the four different radii 0.5, 1, 2, and 4. Plot your results. Make sure your neurons have the same (relative, i.e., scaled by the radius) x-intercepts and maximum rates across all experiments.

🖈 Nengo will automatically rescale the intercepts as the radius increases, so you don’t have to worry about changing the intercepts as you had to in Assignment 3.

🖈 To ensure that you are using the same neuron parameters, just fix the random seed before running the experiment, i.e., by passing a constant to the nengo.Network constructor.

[0.5] c) Discussion. What mathematical relationship between the radius and the RMSE do you observe (write down an equation)? Explain why this is the case.

[0.5] d) RMSE and refractory period. What happens to the RMSE and the tuning curves as τref changes between 1ms to 5ms? Plot the tuning curves for at least four different τref and produce a plot showing the RMSE over τref. Again, make sure to use the same neuron ensemble parameters in all your trials.

[0.5] e) RMSE and membrane time constant. What happens to the RMSE and the tuning curves as τRC changes between 10ms to 100ms? Plot the tuning curves for at least four different τRC and produce a plot showing the RMSE over τRC. Again, make sure to use the same neuron ensemble parameters in all your trials.

[0.5] f) Discussion. Discuss the last two results. Describe what happens to the tuning curves as τref and τRC change (you do not need to come up with a mathematical relationship here). Explain why the change in tuning curve shape influences the RMSE in the way you observe.

2 Connecting neurons

Make a second ensemble of spiking neurons. It should have the same parameters as the first ensemble of neurons (from the first question), but have only 50 neurons in it. Connect the first ensemble to the second such that it computes the identity function, using a post-synaptic time constant of 10ms. Use a synaptic filter of 10ms for your probes. Create a step-function input that is a value of 1 for 0.1 &lt; t &lt; 0.4 seconds, and otherwise is zero.

🐍 You must use a Nengo Node object to feed an arbitrary Python function into a Nengo network. You can use a Python lambda to write this in a very concise way. For example nd_input = nengo.Node(lambda t: 0.0 if t &lt; 0.5 else (1.0 if t &lt; 1.0 else 0.0))

will create a step function that is 1 for 0.5 &lt; t &lt; 1.0 and 0 otherwise. Instead of using a lambda, you can also use the Piecewise process built into Nengo:

nd_input = nengo.Node(nengo.processes.Piecewise({

0.5: 1.0,

1.0: 0.0

}))

[1] a) Computing the identity function. Show the input value and the decoded values from the two ensembles in three separate plots. Run the simulation for 0.5s.

[0.5] b) Computing an affine transformation. Make a new version of the model where instead of computing

the identity function, it computes y(t) = 1 − 2x(t). Show the same graphs as in part (a).

3 Dynamics

Build a neural integrator. This consists of one ensemble, one input, a connection from the input to the ensemble, and a connection from the ensemble back to itself. The ensemble should have 200 neurons and the same parameters as in question 1.

Important: Use two different time constants in your network. The post-synaptic time constant of the recurrent connection is τ = 50ms, and the post-synaptic time constant of the input is 5ms. Having two different time constants violates what we assumed for deriving principle three; use the longer time constant τ (i.e., τ from the recurrent connection) when computing A′ and B′. Part of this assignment is to explore how having two different time constants affects the quality of the result compared to what we saw in the lecture.

🖈 To be an integrator, the desired dynamical system is d , where x is the state of the system and u is the input.

🖈 For all probes, use a synapse of 10ms.

[0.5] a) Transforming the dynamical system. Rewrite the linear dynamical system describing the integrator in terms of d Ax+Bu, i.e., write down the matrices A and B (you can just use the equations from class, you do not have to re-derive the equations) What are the matrices A′ and B′ we have to use

when implementing this system using the recurrent connection post-synaptic filter?

[0.5] b) Integrator using spiking neurons. Show the input, the ideal integral, and the value represented by the

ensemble when the input is a value of 0.9 from t = 0.04 to t = 1.0 (and 0 for other times). Run the simulation for 1.5s.

🖈 For this and the following questions, we consider the scalar case, i.e., the dimensionality n of x and u is one.

🐍 We’re going to run this simulation with various input functions and ensemble parameters in the following questions. It is highly recommended that you write a function that takes ensemble parameters and the input function as arguments and produces all plots you need.

[0.5] c) Discussion. What is the expected ideal result, i.e., if we just mathematically computed the integral of the input, what is the equation describing the integral? How does the simulated output compare to that ideal?

🖈 When you write down the integral of the step function, you have to distinguish between three cases. Your function should be a definite integral of the form

,

🖈 Make sure you understand the difference between a definite and an indefinite integral, before you continue to answer this question.

🖈 Plot the ideal on top of your simulation result in your answer for the previous question.

🐍 You can use the numpy function np.cumsum to compute the ideal integral numerically (don’t forget to scale by dt). However, still write down the integral mathematically to answer this question.

[0.5] d) Simulation using rate neurons. Change the neural simulation to rate mode. Re-run the simulation in rate mode. Show the same plots as in the previous question.

🐍 Pass the extra parameter neuron_type = nengo.LIFRate() to the Ensemble constructor to switch an ensemble to rate mode.

[0.5] e) Discussion. How does this compare to the result in part (b)? What deviations from the ideal do you still observe? Where do those deviations come from?

[0.5] f) Integration of a shorter input pulse. Returning to spiking mode, change the input to be a value of 0.9

from t = 0.04 to 0.16. Show the same plots as before (the input, the ideal, and the value represented by the ensemble over 1.5s).

[0.5] g) Discussion. How does this compare to (b)? What is the ideal equation? Does it work as intended? If not, why is it better or worse?

[0.5] h) Input ramp. Change the input to a ramp input from 0 to 0.9 from t = 0 to t = 0.45 (and 0 for t &gt; 0.45).

Show the same plots as in the previous parts of this question.

[0.5] i) Discussion. What does the ensemble end up representing, and why? What is the (ideal) equation for the curve traced out by the ensemble?

🖈 As above, make sure to write down the definite integral . This means that there will be no integration constant in your result.

[0.5] j) Sinusoidal input. Change the input to 5sin(5t). Show the same plots as before.

[0.5] k) Discussion. What should the value represented by the ensemble be? Write the equation. How well does it do? What are the differences between the model’s behaviour and the expected ideal behaviour and why do these differences occur?

🖈 Again, write down the definite integral . There is no integration constant.

[+1] l) 🌟 Bonus question. Implement a nonlinear dynamical system we have not seen in class (and that is not in the book). Demonstrate that it’s working as expected.

(i) write down the differential equation of the nonlinear system,

(ii) write down the transformed equations that implement the system using the post-synaptic

filter,

(iii) implement the system in Nengo using spiking neurons,

(iv) show that the simulation results match the expected system behaviour at least qualitatively.
