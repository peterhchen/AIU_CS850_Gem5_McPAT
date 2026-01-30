Topics:
1. Power Modeling: We discuss the idea behind Power Model
a. Gem5 has a generic power model that we have define a couple of functions: getDynamicPower () and getStaticPower ().
b. Every SimObject can have a power model. We can have power models for different power states. We can have power model for the ON state, a power model for the off state, a Power model for clock gated state, SRAM retention state, etc.  
2. class MathExprPowerModel in ~/gem5/src/sim/MathExprPowerModel.py: We use Power Model in Gem5.
3. L3 Cache Power Model
4. Power Model Example: three_level.py
5. Test Power Model: test-cache.py
6. Run test-cache.py
7. Check stats.txt and search for keyword “power”, “power_model”, and “dynamic_power
