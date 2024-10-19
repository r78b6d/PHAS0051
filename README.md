java cPHAS0051 Data Analysis Problem Sheet 2024/25 Four questions totalling 42 marks
Submission deadline 5pm, Monday 21st October.
SoRA submission deadline 5pm, Wednesday 30th October.
Submission via Turnitin assignment links on PHAS0051 Moodle page ->Assessment tab.
Please make sure you convert all files to pdf before submitting and check that your file is readable.
You may use spread sheets or programs in the calculations, but you should explain your workings briefly (including equations used). If you are using Python then add clear text comments to your answer and submit a pdf not an executable program. An Excel spreadsheet is a convenient method for χ2 calculations (use Solver for minimising).
A useful resource for answering the problem sheet is the book “Measurements and their Uncertainties” by Hughes and Hase, (See Chapter 8 for hypothesis testing and degrees of freedom). An e-book link is available on the PHAS0051 Moodle overview page
Please make sure you read each question fully including any footnotes See the UCL Academic Manual for late submission penalties.
The use of AI is prohibited.
PHAS0051: Data Analysis Problem Sheet 2024/25
      NN 1/10/2024 Page 1

1. Mean, Variance, Standard Deviation, Standard Error on the Mean and Confidence Limits [10 Marks]
UK climate records are held at the Met Office and are available at the following website:
http://www.metoffice.gov.uk/public/weather/climate-historic/#?tab=climateHistoric
Data has been taken from this website and is presented in appendix I. The data refers to tmin (C), tmax (C), amount of rain (mm) and sunlight (hours) for the month of August, dating from 1911-2023 for the station Bradford.
i. From this data set calculate separately the mean, variance, standard deviation and standard error on the mean for both tmax and tmin over the period 1911-2022. [3]
ii. Estimate the 60% and 90% confidence limits for tmax and tmin for the period 1911- 2022. Assume the distributions are Gaussian. [3]
iii. By considering tmax and tmin for the periods 1911-1922 and 1995-2022, discuss whether there is evidence of global warming in Bradford. [4]
2. Linear fit and 𝛘𝟐 [10 Marks] An experiment is performed to test whether the current through a semiconductor device I,
depends linearly on the potential drop across it, V. The following data are obtained. V/volts 0.20 0.40 0.60 0.80 1.00 1.20 1.40 1.60 1.80 2.00 2.20
I/mA 4.10 5.15 6.11 7.31 8.53 9.90 11.22 12.69 14.21 15.77 17.60 The current measurements are estimated to have the same uncertainty (𝑑𝐼 = ±0.20𝑚𝐴),
whilst the potential drop (V) is estimated to be without significant uncertainty.
i. Using an appropriate program, least squares fit the data to a straight line. [3]
ii. Calculate the 𝜒2 probability for the fit. [3]
iii. On the same graph, plot the data with uncertainty bars and the best fit line and comment on the outcome of the experiment in light of the 𝜒2 probability calculated in part ii and the graphical comparison of the best fit line and the data.
[4]
PHAS0051: Data Analysis Problem Sheet 2024/25
                                        NN 1/10/2024 Page 2

3. Poisson Distribution and 𝛘𝟐 [12 Marks]
The following are results from an experiment in which a Geiger counter is used to record the number of particles emitted per second by a weak radioactive source. In 496 repeated observations for a 1 second interval, counts are recorded with the following f代 写PHAS0051、C++，Java
代做程序编程语言requency:
Counts 0 1 2 3 4 5 6 7 8 9 10 11 12 13 ≥14 Frequency 1 3 11 38 54 79 77 65 60 39 28 17 13 8 3
i. Calculate the mean number of counts per second (μ), the variance and the standard deviation. [3]
ii. Using the values for the mean found in (i) calculate the theoretically expected Poisson frequencies for each number of counts. [3]
iii. Calculate the χ2 probabilities P(χ2) that the frequency distributions follow the expected Poisson distributions with the means you have determined. You can approximate the error on each frequency N, by a Gaussian with standard deviation √N (See Note 2  3 at the end of this question). [4]
iv. Plot both the experimental data and theoretical Poisson distributions. [2]
The Poisson distribution is given by:
P(r) = μre−μ r!
Where, r is the frequency and μ is the mean number of counts.
Note 1: the approximation that the distribution of each Poisson frequency is a Gaussian with standard deviation √𝐍 is a poor one for small N (less than 5 - see Hughes and Hase,
p111 Ch8.6). In order to make the approximation reasonable when comparing the above distribution with theory, the contents of adjacent bins may be summed to give sufficiently large frequencies.
Note 2: the probability 𝐏(𝛘𝟐) is such that 𝟏 − 𝐏(𝛘𝟐) is the probability that the value of 𝛘𝟐 is as low, or lower than the calculated value of, 𝛘𝟐. So a value of 𝐏(𝛘𝟐) very close to unity means an improbably good fit – perhaps too many parameters have been used in the fit, or the uncertainties are underestimated.
PHAS0051: Data Analysis Problem Sheet 2024/25
      NN 1/10/2024 Page 3

4. Best fit by Minimising 𝝌𝟐 [10 Marks]
An experiment is carried out where the voltage, VC, across the capacitance in a resonant series LCR circuit is measured as the frequency f, (ω is the angular frequency) is varied through resonance. The following estimates of the voltage versus frequency are obtained.
PHAS0051: Data Analysis Problem Sheet 2024/25
       f (kHz)
                                                       The uncertainty in the voltage is +/- 0.15V, the frequencies are without uncertainty. According to AC theory the voltage is predicted to vary as:
𝑉𝑐 = 𝐸0
𝐶(𝜔2𝑅2 + 𝐿2(𝜔2 − 𝜔02)2)12
Vc (volts)
28.41 24.11 20.91 18.45 16.25 14.57 13.13 12.01 11.12 9.97
significant
 Where E0 is the amplitude of the AC voltage applied across the circuit which is measured to be 12 volts and L and C are the inductance and capacitance in the circuit having the values 30mH and 950pf. The inductance and capacitance are high precision components and the uncertainties on their values are negligible as is the value of the uncertainty on E0. ω0 is the natural frequency of the freely oscillating circuit with zero damping such that;
𝑅=0,𝜔0= 1 √𝐿𝐶
R in the circuit is only nominally known since it is made up of a resistance box set to 800Ω and an additional smaller contribution due to hysteresis losses in the core of the inductor.
i.
ii.
iii.
By minimising the 𝜒2 fit of the data to the theoretical form, estimate the best value for the total resistance in the circuit and the additional resistance due to hysteresis [5]
What is the 𝜒2 probability for the best fit and does this value support the AC theory given above? [3]
Plot a graph and comment on the agreement / disagreement between the data and fitted curve [2]
  NN
1/10/2024 Page 4

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
