Final Insights Summary

1. Hydraulic pressure is the strongest indicator of machine failure
Normal operation: median ≈ 120 bar
Failure events: median ≈ 78 bar
Correlation with failure: –0.56
Highest feature importance in Random Forest

Conclusion:
A drop in hydraulic pressure is the clearest early warning of an upcoming failure.

2. Cutting force increases significantly during failure
Failure cutting force: ≈ 2.85 _ 3.60 kN
Normal cutting force: ≈ 2.50 _ 3.00 kN
Correlation: +0.45
High feature importance

Conclusion:
High cutting force under weak pressure creates the most stressful operating condition.

3. Torque and load index both decrease before failures
Failures occur at lower torque and lower load index
Correlation around -0.40

Conclusion:
The machine loses its ability to carry load just before failing.

4. Certain variable interactions explain over 80% of failures
Most critical combinations:
Interaction	                                            Failure Probability
Low hydraulic pressure + high cutting force	                 0.82
High coolant temperature + low hydraulic pressure	         0.85
Low hydraulic pressure + low torque	                         0.79

Conclusion:
Hydraulic pressure amplifies the effect of every other variable.
When pressure is low, any additional stress almost guarantees a failure.

5. Failures are not caused by machine type
Failure rates:
Makino-L1 → 0.52
Makino-L2 → 0.49
Makino-L3 → 0.50

Conclusion:
All machines behave similarly.
The issue is operational conditions, not the machine design.

6. Time of day and weekday effects are minimal

Wednesday slightly higher
Weekend ≈ Weekday

Conclusion:
Scheduling is not a cause of failure.
Sensor conditions are far more significant.

7. Sensors show noticeable volatility over time
Large fluctuations in:
Hydraulic pressure
Coolant temperature
Spindle speed
Torque
Load index

Conclusion:
The operating environment is unstable during several periods, especially at the beginning and end of the dataset.


Final Insight:
Machine failures are mainly caused by operating under high cutting load while the hydraulic/torque system cannot support the required force.