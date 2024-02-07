- 👋 Hi, I’m @dhiraj525
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
dhiraj525/dhiraj525 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->import numpy as np
import matplotlib.pyplot as plt

# Constants
c = 1  # Speed of light
m0 = 1  # Rest mass

# Range of velocities (from 0 to 0.99c)
velocities = np.linspace(0, 0.99, 100)

# Calculate relativistic mass for each velocity
masses = m0 / np.sqrt(1 - velocities**2)

# Plot
plt.figure(figsize=(10, 6))
plt.plot(velocities, masses, color='blue', label='Relativistic Mass')
plt.xlabel('Velocity (c)')
plt.ylabel('Mass (m)')
plt.title('Variation of Mass with Speed (Lorentz Transformation)')
plt.grid(True)
plt.legend()
plt.show()
