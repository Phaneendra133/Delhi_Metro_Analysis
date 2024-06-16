# Delhi_Metro_Analysis
Delhi Metro Analysis using Pyspark and matplotlib.


# Delhi Metro Network Analysis

This repository contains the analysis of the Delhi Metro Network dataset, which includes information on 285 stations. The dataset provides details such as Station ID, Station Name, Distance from Start (km), Line, Opening Date, Station Layout, Latitude, and Longitude.

## Dataset Summary

The dataset contains the following columns:
- `Station ID`: Integer (nullable = true)
- `Station Name`: String (nullable = true)
- `Distance from Start (km)`: Double (nullable = true)
- `Line`: String (nullable = true)
- `Opening Date`: Date (nullable = true)
- `Station Layout`: String (nullable = true)
- `Latitude`: Double (nullable = true)
- `Longitude`: Double (nullable = true)

### Statistical Overview

|   | Station ID | Station Name | Distance from Start (km) | Line | Station Layout | Latitude | Longitude |
|---|------------|--------------|--------------------------|------|----------------|----------|-----------|
| **Count** | 285 | 285 | 285 | 285 | 285 | 285 | 285 |
| **Mean** | 143.0 | NULL | 19.22 | NULL | NULL | 28.60 | 77.03 |
| **Stddev** | 82.42 | NULL | 14.00 | NULL | NULL | 0.09 | 2.88 |
| **Min** | 1 | AIIMS | 0.0 | Aqua line | At-Grade | 27.92 | 28.70 |
| **Max** | 285 | Yamuna Bank | 52.7 | Yellow line | Underground | 28.88 | 77.55 |

### Key Insights

- **Extensive Network**: The Delhi Metro covers a broad area with significant variations in distances from the start point, indicating its reach across the city and outskirts.
- **Diverse Station Layouts**: The network includes both at-grade and underground stations, catering to different geographical and infrastructural requirements.
- **No Underground Stations on Red Line**: All stations on the Red Line are elevated, with no underground tunnels.

### Distance Conversion

The distance from the start point was converted from kilometers to miles and the column was renamed to `Distance Miles`.

## Line-Specific Analysis

| Line | Average Distance (miles) | Maximum Distance (miles) |
|------|--------------------------|--------------------------|
| Rapid Metro | 3.55 | 6.21 |
| Blue Line | 16.25 | 32.75 |
| Green Line Branch | 0.66 | 1.30 |
| Green Line | 7.07 | 15.41 |
| Blue Line Branch | 2.49 | 5.03 |
| Violet Line | 12.81 | 27.03 |
| Yellow Line | 13.34 | 28.40 |
| Gray Line | 1.12 | 2.42 |
| Red Line | 10.29 | 20.32 |
| Pink Line | 17.88 | 32.68 |
| Magenta Line | 10.97 | 20.57 |
| Orange Line | 6.57 | 12.92 |
| Aqua Line | 8.30 | 16.84 |

### Notable Observations

- **Long-Distance Travel**: The Blue Line and Pink Line stand out for their long maximum distances, making them crucial for long-distance travel.
- **Localized Transit**: Lines like Rapid Metro, Green Line Branch, and Gray Line focus on addressing specific, localized transit needs in addition to broader city-wide connectivity.



The line graph provided shows the number of stations per line in the Delhi Metro Network. Here are some useful insights based on the graph:

1. **Blue Line Dominance**: The Blue Line has the highest number of stations, reaching nearly 50. This indicates that the Blue Line is a major artery in the Delhi Metro network, covering a significant portion of the city.

2. **Variation in Line Coverage**: There is a significant variation in the number of stations across different lines. Some lines, like the Green Line Branch and Gray Line, have very few stations, suggesting they serve specific, localized areas or act as short extensions to other lines.

3. **Prominent Lines**: Besides the Blue Line, the Pink Line and Yellow Line also have a substantial number of stations, indicating their importance in providing extensive coverage across the city.

4. **Smaller Lines**: The Rapid Metro, Blue Line Branch, and Aqua Line have fewer stations, reflecting their more targeted coverage or possibly serving less populated or smaller regions.

5. **Key Insights for Urban Planning**:
   - **High Station Density Areas**: Areas served by the Blue Line, Pink Line, and Yellow Line likely have higher accessibility and connectivity due to the higher number of stations.
   - **Targeted Expansion**: Lines with fewer stations, such as the Gray Line and Green Line Branch, may be targets for future expansion to increase connectivity and reduce travel times for commuters in those areas.

**Most number of metro stations are located on elevated layouts followed by underground station layouts with least number of stations located at the ground level.**
**Most number of metro stations were opened in the year 2005 followed by 2019 and 2018. The first metro station was opened in the year 2002. No metro statio were opened in the years 2007, 2012, 2016.**

