<h1><b>TI-84 Evo Programs</b2></h1>

- <h3><i>MINROOT</i></h3> 

  - Find the minimum root of a given value under a radical.
  - <code>Sqrt(X), X=27 ➡️ 3 * sqrt(3)</code>
- <h3><i>FACTOR</i></h3> 

  - Find factors of X. 
  - <code>27 ➡️ {1,3,9,27}</code>
- <h3>MOD</h3> 

  - Calc Modulus of X. Useful for finding co-terminal values.
  - <code>295, 180 ➡️ 115</code> 
- <h3>PIRATIO</h3> 

  - Find the exact pi ratio of a given decimal approximation.
  - <code>X = 1.832595715 (represents 7pi/12)</code>
  - <code>1.832595715 ➡️ 7pi/12</code>
- <h3>ROOTMATC</h3> 
  
  - Find an exact root that matches a decimal value approximation.
  - <code>X=5.360475154 (represents 8*sqrt(22)/7 )</code>
  - <code>5.360475154 ➡️ 8 * sqrt(22)/7</code>

<h3>TI-84 Evo Links:</h3>

Online Calculator (login realityexpander)
  - https://ti84evo.ti.com/84evo/en/main-view
  - Use "Send Files" - "send to calculator" to send a program file on computer to a the emulator calculator.
  - Use "Send Files" - "send to computer" to copy a program from the emulator calculator to your computer files.

Connect to Physical Calculator
  - https://connectevo.ti.com/ticevo/en/main-view
  - Use "send to calculator" to send a program file to a physically connected calculator.
  - Use "send to computer" to copy a program from the physical connected calculator to your computer files.

Convert Text File BASIC code to TI-BASIC Encoded file
  - Use TI-CONNECT CE, paste in code, save as .8xp
  - OR... Use TI-Basic Program Converter @ https://tiplanet.org/scripts/EvoConv/
    - Paste in the text, save as .8xp or .8xp2

Convert Text File Python to TI-Python, no need to encode, programs are stored as plain text
  - Use TI Connect Evo, simply upload to calculator

TI 84 <-> TI-84 EVO TI-BASIC Program Converter (.8xp2 <-> .8xp)
  - https://tiplanet.org/scripts/EvoConv/

Alternative TI-BASIC Converter
  - https://www.cemetech.net/sc/

<h1><b>TI-NSpire CX-II NON-CAS Programs</b2></h1>
<h2>Programs for Pre-calculus on the TI-NSpire CX II (NON-CAS). Adds some functionality from CAS calculator, like converting decimals to exact values and ratios of pi, useful for confirming hand-written work on tests and quizzes, if your professor allows use of this NON-CAS calculator.</h2>
<h3><i>compint</i>: Compute Interest / Decay / Compound Interest </h3>

- <code>compint(prin,rate,period,time)</code> - compute interest given principal, rate, period, time
- <code>contcompint(prin,rate,time)</code> - compute continuously compounding interest given principle, rate, time
- <code>expdecay(init,half_life,time)</code> - compute exponential decay given Initial Amount, Half life (years), time (years)
- <code>expgrow(init,growth,time)</code> - Compute exponential growth given initial amount, growth (in a period), time (periods)

<h3><i>cvt_degs_rad</i>: Convert degrees to radians and radians to degrees, reference angles</h3>

- <code>to_degrees(x)</code> - Convert x radians to degrees, ie: (r * 180) / pi
- <code>to_radians(x)</code> - Convert x degrees to radians, ie: (d / 180) * pi
- <code>to_ref_angle(x)</code> - Convert x degrees to reference angle in Quadrant I
- <code>to_ref_rad2(n,d)</code> - Convert pi ratio radians (Numerator w/o pi, Denominator) to reference angle radians in Quadrant I
- <code>to_ref_rads(x)</code> - Convert x radians to reference angle radians in Quadrant I 

<h3><i>exacts</i>: Find the exact values based on decimal approximations within an error range.</h3>

- <code>exact_pi(x)</code>
  - Convert decimal approximation of a pi ratio to an exact pi ratio, x < 50*pi/50
  - <code>ex: exact_pi(4.9367884556411) ➡️ {11, "π", "/", 7}      ie: (11π/7) </code>
- <code>exact_pi2(x)</code>
  - Improved exact_pi, convert decimal approximation of a pi ratio to an exact pi ratio, x < n*pi/1000
  - <code>ex: exact_pi(4.9367884556411) ➡️ {11., "π/", 7.}     ie: (11π/7) </code>
- <code>exactsq(x)</code>
  - Find the exact square value given a decimal value x, max ( ((20 * sqrt(100)) / (20) )
  - <code>ex: exactsq(10.392304845413) ➡️ {6., "√", 3, "/", 1 }     ie: (6√3)</code>
- <code>minroot(x)</code>
  - Given a value x under a radical, find the minimum root value. Ex: sqrt(27) -> x=27
  - ex: <code> minroot(27) ➡️ {3, "√", 3} which means 3√3</code>
- <code>nest_rad(a,b,c)</code> - Given coefficients under a nested set of radicals, reduce to two separate radicals.
  - √( (a ± √b) / c)  ➡️  (√x ± √y)/c 
  - ex: (sqrt(2 + sqrt(3)))/4, nest_rad(2,3,4)   ➡️  (√6 ± √2)/4
 
<h3><i>factors</i>: Finds factors of a integer.</h3>

- <code>facts(constant,lead_coeff)</code> - Gives all factors for a an equation, given the leading coefficient and ending constant, used to find roots of a complicated equation (usually above order 2), and finding an initial divisor for synthetic division.
  - <code>3*x^(3)-6*x^(2)-57*x+60,  constant (num)=60, lead_coeff (denom)=3
  -  facts(60,3) ➡️
    - +/- {1,2,3,4,5,6,10,12,15,20,30,60}   (factors of numerator)
      +/- {1,3}                             (factors of denominator)
      {"±",1/3,2/3,1,4/3,5/3,2,3,10/3,4,5,6,20/3,10,12,15,20,30,60}  (ascending list of factor ratios) </code>
  - One of these values will be a root of the equation 3*x^(3)-6*x^(2)-57*x+60, and a start divisor value for synthetic division.
- <code>findfact(sum,product)</code>
  - Given a simple quadratic formula, ie: x^2 + 3*x - 28, find the two factors for the two unexpanded source equations:
  - ex: <code>sum=3, product=-28, findfact(3,-20) ➡️   {−4,7} means the two unexpanded source equations are: (x-4)(x+7) for: x^2+3*x-28</code>
- <code>quadrat(a,b,c)</code>
  - Similar to polysolve, finds constants and coefficients for quadratic equations.
  - ex:<code> x^(2)+3*x-28, quadrat(1,3,−28)   ➡️  {−3,"±",11,"ℝ","/",2,"→",4,−7}</code>
    - which means: (x-4)(x+7), which has roots at x=4, x=-7  

<h3><i>law_of_cos</i>: Using the law of cosines, compute triangle values for various kinds of triangles.</h3>

- These could possibly solved better using the nsolve command (in DEG mode): 
  - ex:<code>nSolve(c^2=a^2+b^2-2*a*b*cos(cd),cd)|a=3 and b=4 and c=5   ➡️   ad=90</code>
- <code>law_of_cos_sas(side_a, ang_c, side_b)</code>
  - Computes side C length. ang_c is in degrees and does not require DEG mode. 
  - ex: <code> law_of_cos_sas(3,90,4)   ➡️  5 </code>
- <code>law_cos_sss(side_a, side_b, side_c)</code>
  - Computes angle A (opposite side_a) in DEGREES.
  - ex: <code> law_of_cos_sss(3,4,5)   ➡️  36.8699° </code>
- semi_perim(side_a,side_b,side_c)</code>
  - Computes semi-perimeter =(a+b+c)/2
  - ex: <<code> semi_perimeter(3,4,5)   ➡️  6 </code>
- <code>solve_ass(ang_a, side_a, side_b)</code>
  - Computes triangle data for 0, 1, 2 triangle cases for SSA triangles.
  - Outputs the 1st & 2nd triangle angles, A, B, C, and length a, b, c.
  - ex: <code> law_of_cos\solve_ass(60,14,15)    ➡️
    [["1△°A,B,C",60,68.107391093321,51.892608906679]
    ["1 len a,b,c",14,15,12.720153254454]
    ["2△°A',B',C'",60,111.89260890668,8.10739109332]
    ["2 len a',b',c'",14,15,2.2798467455463]] </code>
- tri_area(side_a,side_b,side_c)</code>
  - Computes area of triangle, s=semi-perimiter,  =sqrt(s*(s-side_a)*(s-side_b)*(s-side_c))
  - ex: <code> tri_area(3,4,5)   ➡️  6 </code>
