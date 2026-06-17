#Debug Test Data Generator

A free web tool for generating randomized compaction test field data. No installation, no server, no account required — just open the link and use it. Used for debugging purposes on Excel files. Use by your own risk.

**Live at [shotgen.site](https://shotgen.site)**

---

## What it does

Generates pseudo-random **Dry Density (pcf)** and **Percent Moisture (%)** values for up to three materials, and outputs a formatted `.xlsx` file matching a standard compaction test field data template.

Values are distributed according to real-world compaction behavior:
- Weight values stay within your specified compaction limits
- Moisture values are distributed relative to optimum moisture
- Higher weight readings are correlated with moisture values closer to optimum (~60% of the time)
- Outliers are rare and statistically controlled

---

## How to use

1. Select how many materials (1, 2, or 3)
2. Enter parameters for each material:
   - Optimum Moisture (%)
   - Max Dry Weight (pcf)
   - Moisture Lower and Upper offsets
   - Compaction Lower and Upper limits (% of Max Weight)
3. Set the number of rows to generate (up to 363)
4. Adjust tightness sliders to control how spread out values are
5. Click **Generate & Download Excel**

---

## Parameters explained

| Parameter | Description |
|---|---|
| Optimum Moisture | Target moisture value for the material |
| Moisture Lower Limit | Offset below optimum that defines the lower bound (e.g. 2 = Optimum − 2%) |
| Moisture Upper Limit | Offset above optimum that defines the upper bound (e.g. 2 = Optimum + 2%) |
| Max Dry Weight | Maximum achievable dry density (pcf) for the material |
| Compaction Lower Limit | Minimum acceptable compaction as % of Max Weight |
| Compaction Upper Limit | Maximum acceptable compaction as % of Max Weight |
| Weight Tightness | Controls how tightly weight values cluster within compaction limits |
| Moisture Tightness | Controls how tightly moisture values cluster within moisture limits |

---

## Output

A `.xlsx` file formatted to match the standard compaction field test template, with:
- Material parameters filled in the header section
- Generated data rows for each active material
- Multiple materials placed side by side as separate column sets

---

## Offline use

The tool is fully self-contained. Download `index.html` and open it in any browser — no internet connection required.

---

## License

MIT License — © Daniel Carens
