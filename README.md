Note: This is a case study exercise. The dataset is completely synthetic/dummy
data created to match the structure of an executive reporting dashboard I build
professionally. The technical approach, data model design, and DAX logic are authentic.

**What I did:**
- Imported distributor performance data into Power BI
- Created KPI cards tracking Sales, Total Distributor, and Active Distributor counts
- Built a segmented breakdown table by distributor tier (New Member, Standard
  Distributor, etc.)
- Added Previous Month and Previous Year comparison values next to every
  current-period metric, so short-term and long-term trends are visible at a glance
- Included variance % (color-coded) on all comparisons for quick visual read
- Implemented filters/slicers for interactive exploration (Country, Year, Month)
- Designed a single-page executive summary layout for quick-scan reporting

## Dashboard Structure:

- Single-page executive summary layout (the original professional dashboard
  spans multiple pages; this portfolio version focuses on one page for
  demonstration purposes)
- Cross-filtering using slicers (Country, Year, Month Name)
- Consistent color scheme and visual hierarchy (green/red KPI cards)

## Visualizations:

- KPI cards with dual metrics (absolute values + % variance)
- Segment breakdown table (Count, Active, Activity %, Sales, Productivity)
- Conditional formatting (green/red) on variance chips for visual emphasis
- Prior Month (PM) and Prior Year (PY) comparison chips on every metric

## Data Handling:

- Imported synthetic distributor and transaction data with distributor-level granularity
- Created calculated measures for rate-based metrics (e.g.,
  `Activity % = Active Distributor / Total Distributor`)
- Structured data to enable filtering by Country, Year, Month

## Interactivity:

- Implemented slicer-based filtering (Country, Year, Month Name)
- Set up visual-to-visual interactions (filtering updates all related cards/tables)

## Design Decisions:

- Chose a segmented table layout (over separate charts) to allow side-by-side
  comparison of all metrics across distributor tiers
- Used conditional color formatting (green ↑ / red ↓) for instant visual read
  on variance direction
- Placed top-level KPIs at the top for executive-level quick scan
- Included both Prior Month and Prior Year comparisons on every row, so
  short-term and long-term trends are visible without switching views

## Tools used:
Power BI · DAX · Power Query (M) · Python (mock data generation, assisted by Claude AI)
