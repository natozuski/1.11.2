wool          	35:
glass			95:
clay			82: 
wood planks		5:
stone			1:
obsidian 		49

imagine a minecraft cube. and its 1000x1000x1000, for example.
its filled.
now imagine its mostly filled, randomly with 8 different colours of wool block.
in a random configuration.
and every game tick, for each block, the following is calculated:
1. what are the surrounding blocks (in the whole cube)
2. where should it "go" next (whats the vector)
then at the next game tick it makes a decision
thats the G field (gluon field)
so for wool blocks id's, you have 35:0, 35:1, 35:2 - 35:7 (thats 8 in total)

now imagine, superimposed onto that, the same thing
but with 3 different colours of glass block.
thats the W field; the weak field.
so it occupies the same space.
so for glass block id's you have 95:0 - 93:2 (thats 3 in total)

now imagine, superimposed onto that, the same thing
but with only 1 colour of obsidian block.
thats the B field; the supercharge field.
so it occupies the same space.
this field is different because at the "game tick decision" stage
it doesnt check what the surrounding blocks are saying.
so the block id is 49

relating this to the gauge terms:
\mathcal{L}_{\text{gauge}}
\enspace &= \enspace
-\frac{1}{4}(\partial_\mu G_\nu^a - \partial_\nu G_\mu^a)(\partial^\mu G^{a\nu} - \partial^\nu G^{a\mu}) \\
&- \qquad 											%
\frac{g_s}{2} f^{abc} (\partial_\mu G_\nu^a - \partial_\nu G_\mu^a) G^{b\mu} G^{c\nu} \\
&- \qquad											%
\frac{g_s^2}{4} f^{abc} f^{ade} G_\mu^b G_\nu^c G^{d\mu} G^{e\nu} \\
&- \enspace											%
\frac{1}{4}(\partial_\mu W_\nu^i - \partial_\nu W_\mu^i)(\partial^\mu W^{i\nu} - \partial^\nu W^{i\mu}) \\
&- \qquad											%
\frac{g}{2} \epsilon^{ijk} (\partial_\mu W_\nu^i - \partial_\nu W_\mu^i) W^{j\mu} W^{k\nu} \\
&- \qquad											%
\frac{g^2}{4} \epsilon^{ijk} \epsilon^{ilm} W_\mu^j W_\nu^k W^{l\mu} W^{m\nu} \\
&- \enspace											%
\frac{1}{4}(\partial_\mu B_\nu - \partial_\nu B_\mu)(\partial^\mu B^\nu - \partial^\nu B^\mu)


you start with a specific field configuration. 
this is called the initial state. 
its a "storyboard"; an arrangement of blocks, a random one, for all of time from time 0 to time N.
what youre trying to figure out, is the "chance" that your storyboard will evolve from time 0's state to time N's state.
from the initial tick's to the final tick's state.
you pick a block from a specific point on that storyboard. so maybe block 500,500,500. from tick 0.
then you calculate what will happen from tick 0 onwards, locally to that block, using all the gauge terms.
then you get your "cloud of blocks", which is a 'guess' at what will happen to those surrounding blocks at the final tick.
you are interested at what happens at the end of ticks.
so youve calculated a guess at what will happen at the final tick.

then you calculate S, by integrating the guess' cloud of blocks with respect to the rest of the storyboard for those cloud of blocks' blocks. which basically means calculating how far off your term-calculated guess is from the storyboard's natural evolution at the final tick.
instead of a guess lets call it a futurecast.
the result is a single number, S. it represents the difference between the futurecast and the storyboard at the final tick.
lets say its 42

then you so e^(iS/h) (where h is reduced plank's constant; just a constant). and this gives you a new number called a phase.
then you literally repeat this whole process with new random storyboards, for every single possible storyboard but keeping with the same reference block (so '500,500,500' from tick 0). which will give you all the possible phases.
then you sum all the phases, to give you the 'total amplitude'.
then you square that to give the probablility. which is the probability that at the final tick of your storyboard, block 500,500,500 will be what you thought it was.

you can see why its a lagrangian😆 its like saying "whats the chance my plan will work and not be disuaded by the (FIXED) fluctuations of gauge fields" 
