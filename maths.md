System of the heat partial differential equation

$$\frac{\delta T}{\delta t} = \alpha ( \frac{\delta^{2}T}{\delta^{2}x} + \frac{\delta^{2}T}{\delta^{2}y})$$

Solve with Explicit Euler's methode

Approximation temporal derivative

$$ \frac{\delta T}{\delta t} \approx \frac{T^{n+1}_{i,j} - T^{n}_{i,j}}{\Delta t}  $$

Approximation spatial derivative

$$ \frac{\delta^{2}T}{\delta^{2}x} \approx \frac{T^{n+1}_{i+1,j} - 2 T^{n}_{i,j} +T^{n+1}_{i-1,j} }{(\Delta x)^{2}}$$

$$ \frac{\delta^{2}T}{\delta^{2}} \approx \frac{T^{n+1}_{i,j+1} - 2 T^{n}_{i,j} +T^{n+1}_{i,j-1} }{(\Delta y)^{2}}$$



Discretized heat equation
$$ \frac{T^{n+1}_{i,j} - T^{n}_{i,j}}{\Delta t} = \alpha (\frac{T^{n+1}_{i+1,j} - 2 T^{n}_{i,j} +T^{n+1}_{i-1,j} }{(\Delta x)^{2}} + \frac{T^{n+1}_{i,j+1} - 2 T^{n}_{i,j} +T^{n+1}_{i,j-1} }{(\Delta y)^{2}}) $$

Solution future temperature
$$T^{n+1}_{i,j} = T^{n}_{i,j} + \Delta t . \alpha(\frac{T^{n+1}_{i+1,j} - 2 T^{n}_{i,j} +T^{n+1}_{i-1,j} }{(\Delta x)^{2}} + \frac{T^{n+1}_{i,j+1} - 2 T^{n}_{i,j} +T^{n+1}_{i,j-1} }{(\Delta y)^{2}}) $$
