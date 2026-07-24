<h2><b>TI-84 & Evo Programs</b2></h2>

- MINROOT - Find the minimum root of a given value under a radical.
  - Sqrt(X), X=27 ➡️ 3 * sqrt(3)
- FACTOR - Find factors of X. 
  - 27 ➡️ {1,3,9,27}      
- MOD - Calc Modulus of X. Useful for finding co-terminal values.
  - 295, 180 ➡️ 115
          
- PIRATIO - Find the exact pi ratio of a given decimal approximation.
  - X = 1.832595715 (represents 7pi/12)
  - 1.832595715 ➡️ 7pi/12
          
- ROOTMATC - Find an exact root that matches a decimal value approximation.
  - X=5.360475154 (represents 8*sqrt(22)/7 )
  - 5.360475154 ➡️ 8 * sqrt(22)/7


<h3>TI-84 Evo Links:</h3>

Online Calculator (login realityexpander)
https://ti84evo.ti.com/84evo/en/main-view

Connect to Physical Calculator
https://connectevo.ti.com/ticevo/en/main-view

TI 84 <-> TI 84 EVO Program Converter
https://tiplanet.org/scripts/EvoConv/

Alternative Converter
https://www.cemetech.net/sc/

<h2><b>TI-NSpire Programs</b2></h2>

- compint - Compute Interest / Decay / Compound Interest
  - compint - compute interest given principal, rate, period, time
  - comtcompint - compute continuously compounding interest given principle, rate, time
  - expdecay - compute exponential decay given Initial Amount, Half life (years), time (years)
  - expgrow - Compute exponential growth given initial amount, growth (in a period), time (periods)

- cvt_degs_rad - Convert degrees to radians and radians to degrees, reference angles
  - to_degrees(x) - Convert x radians to degrees,  (r * 180) / pi
  - to_radians(x) - Convert x degrees to radians, (d / 180) * pi
  - to_ref_angle(x) - Convert x degrees to reference angle in Quadrant I
  - to_ref_rad2(n,d) - Convert pi ratio radians (Numerator w/o pi, Denominator) to reference angle radians in Quadrant I
  - to_ref_rads(x) - Convert x radians to reference angle radians in Quadrant I 

- exacts
  - exact_pi(x) - Convert decimal approximation of a pi ratio to an exact pi ratio, x < 50*pi/50
    - x=4.9367884556411 ➡️ {11, "π", "/", 7}      ie: (11π/7) 
  - exact_pi2(x) - Improved exact_pi, convert decimal approximation of a pi ratio to an exact pi ratio, x < n*pi/1000
    - x=4.9367884556411 ➡️ {11., "π/", 7.}     ie: (11π/7)
  - exactsq(x) - Find the exact square value given a decimal value x, max ( ((20 * sqrt(100)) / (20) )
    - x=10.392304845413 ➡️ {6., "√", 3, "/", 1 }     ie: (6√3)
  - minroot(x) - Given a value x under a radical, find the minimum root value. Ex: sqrt(27) -> x=27
    - x=27 ➡️ {3, "√", 3}
  - nest_rad(a,b,c) - Given coefficients under a nested set of radicals, reduce to two separate radicals.
    - √( (a ± √b) / c)  ➡️  (√x ± √y)/c

- factors
  - facts(constant,lead_coeff) - Gives all factors for a an equation, given the leading coefficient and ending constant, used to find roots of a complicated equation (usually above order 2), and finding an initial divisor for synthetic division.
    - 3*x^(3)-6*x^(2)-57*x+60,  constant (num)=60, lead_coeff (denom)=3
    -   ➡️  +/- {1,2,3,4,5,6,10,12,15,20,30,60}   (factors of numerator)
            +/- {1,3}                             (factors of denominator)
            {"±",1/3,2/3,1,4/3,5/3,2,3,10/3,4,5,6,20/3,10,12,15,20,30,60}  (ascending list of factor ratios)
        - One of these values will be a root of the equation 3*x^(3)-6*x^(2)-57*x+60, and a value for synthetic division.
  - findfact - 
  - nest_rad -
  - quadrat -
 
- law_of_cos
  - law_of_cos_ssa -
  - law_cos_sss -
  - semi_perim -
  - tri_area -   

