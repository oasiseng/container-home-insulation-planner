# Shipping Container Insulation Planner

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/yourusername/shipping-container-insulation-planner.svg?style=social)](https://github.com/yourusername/shipping-container-insulation-planner/stargazers)

A sleek, interactive web-based tool to plan insulation for shipping container conversions based on IECC 2021 prescriptive R-values. Select your location to get required R-values for ceiling, walls, and floor, then choose insulation types and thicknesses to visualize compliance with elegant, animated graphics.

**Note:** This is an estimation tool for educational purposes. Always consult local building codes and a licensed professional for actual designs, as requirements may vary by jurisdiction or project specifics.

## Features

- **Location-Based R-Values:** Select U.S. state and climate zone to display IECC-required minimum R-values for ceiling, walls, and floor.
- **Insulation Options:** Choose from Spray Foam (R-6/in), Batt (R-3.5/in), or Polyiso (R-6/in) for each component.
- **Wall Configurations:** Support for cavity-only or cavity + continuous insulation, with inside/outside placement.
- **Real-Time Feedback:** Instant R-value calculations, compliance status (green/red), and smooth visual animations showing insulation layers.
- **Responsive Design:** Modern, minimalist UI that works beautifully on desktop and mobile—visuals scale gracefully.
- **No Dependencies:** Pure HTML, CSS, and JavaScript—lightweight and easy to host.

## Demo

You can try the planner live [here](https://[[oasisengineering.com/shipping-container-insulation-planner/](https://oasisengineering.com/container-home-insulation-planner/)]

## Installation

No installation required! This is a static web page.

1. Clone the repository:
2. Open `index.html` in your web browser.

Alternatively, download the ZIP and open the HTML file directly.

## Usage

1. Select your U.S. state and climate zone to load required R-values.
2. For each component (floor, ceiling, walls):
- Choose insulation type.
- Enter thickness in inches.
- For walls: Select configuration (cavity only or + continuous) and location (inside/outside).
3. Watch real-time updates: Provided R-value, compliance status, and animated visuals depicting insulation layers.
4. Adjust until all statuses are green for compliance.

### Example

- State: California
- Climate Zone: 3B
- Floor: Polyiso, 3.2 inches → R-19.2 (Meets R-19)
- Ceiling: Spray Foam, 6.4 inches → R-38.4 (Meets R-38)
- Walls: Cavity (Batt, 3.8 inches) + Continuous (Polyiso, 0.9 inches), Inside → Cavity R-13.3, Continuous R-5.4 (Meets R-13+5)

Visuals show layered insulation with smooth gradients and subtle animations.

## Technical Details

- **Data Sources:** IECC 2021 R-value tables; state-to-zone mappings based on standard U.S. climate data.
- **Calculations:** Simple R = thickness * R-per-inch; wall compliance parses "or" options like "20 or 13+5".
- **Visuals:** SVG-based with linear gradients for insulation (blue tones), corrugated wall pattern for realism, and CSS transitions for smooth scaling.
- **Limitations:** Assumes basic IECC prescriptive paths; no U-factor alternatives, advanced assemblies, or non-U.S. locations. Walls visualize cavity/continuous as additive layers.

## Contributing

Contributions are welcome! Please fork the repo and submit a pull request.

1. Fork the project.
2. Create a feature branch (`git checkout -b feature/AmazingFeature`).
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the branch (`git push origin feature/AmazingFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Disclaimer

This tool provides estimates based on IECC 2021 prescriptive R-values and is not a substitute for professional advice. Calculations assume standard insulation performance; actual values may vary with installation, materials, and local amendments. Verify with a licensed engineer or building official to ensure compliance with codes and site-specific conditions. Oasis Engineering assumes no liability for any use of this tool.

## Acknowledgments

- Inspired by sustainable shipping container architecture and IECC energy efficiency standards.
- Designed with a focus on simplicity and elegance, à la Steve Jobs' philosophy.

If you find this useful, star the repo! ⭐

https://oasisengineering.com/shipping-container-insulation-planner/ 
