# Human Archive Egocentric Dataset

Composition of the 15,000-hour Human Archive egocentric dataset: first-person video of people doing real work inside businesses
across India, captured with a head-mounted stereo camera (10,000 h) and a multi-camera rig with wrist cameras (5,000 h).
Every clip carries 3D hand keypoints, camera pose, IMU and dense action annotations, plus category, environment, scene and task labels.

Live page: https://samaymaini.github.io/human-archive-dataset/

## At a glance

| | Full dataset | Stereo | Multi-camera + wrist |
|---|---:|---:|---:|
| Hours | 15,000 | 10,000 | 5,000 |
| Clips and recordings | 3,597,783 | 2,635,016 | 962,767 |
| Businesses | 641 | 433 | 350 |
| Operators | 8,999 | 7,246 | 2,797 |
| Categories | 26 | 26 | 25 |
| Environment types | 112 | 82 | 87 |
| Distinct scenes | 5,812 | 3,560 | 2,802 |
| Distinct scene × task pairs | 15,415 | 10,034 | 6,374 |
| Task categories | 27,375 | 7,954 | 20,952 |
| Task descriptions | 920,819 | 449,545 | 471,274 |

## Categories (full dataset)

| Category | Hours | Share |
|---|---:|---:|
| Food and Beverage | 2,203 | 14.7% |
| Sewing and Tailoring | 1,532 | 10.2% |
| Warehousing and Logistics | 1,420 | 9.5% |
| Textiles and Garments | 1,294 | 8.6% |
| Residential | 1,160 | 7.7% |
| Manufacturing | 943 | 6.3% |
| Automobile | 913 | 6.1% |
| Construction | 886 | 5.9% |
| Agriculture and Farming | 842 | 5.6% |
| Printing and Design | 627 | 4.2% |
| Hospitality | 578 | 3.9% |
| Handcraft & Woodwork | 412 | 2.7% |
| Retail Trade | 410 | 2.7% |
| Waste Management | 370 | 2.5% |
| Sanitation Services | 365 | 2.4% |
| Beauty and Grooming | 301 | 2.0% |
| Repair and Servicing | 192 | 1.3% |
| Horticulture | 154 | 1.0% |
| Fitness and Sport | 152 | 1.0% |
| Live Events and Entertainment | 102 | 0.7% |
| Scientific Labs | 63 | 0.4% |
| Energy and Utilities | 40 | 0.3% |
| Offices | 31 | 0.2% |
| Healthcare | 6 | 0.0% |
| Data Centers and Networking | 5 | 0.0% |
| Other | 2 | 0.0% |

## Definitions

- **Category** — the industry the business belongs to.
- **Environment type** — the kind of venue within a category (for example, a cold storage within warehousing and logistics).
- **Distinct scene** — a scene type at one business with at least five minutes of footage. The same kind of scene recorded at a
  different business counts as a new distinct scene.
- **Distinct scene × task pair** — a task category recorded for at least five minutes in a distinct scene. The same pair at a
  different business counts as a new distinct pair.
- **Task description** — the specific activity in a labelled segment; the count is of unique descriptions.
- **Business** — a working site where footage was recorded (every business with footage is counted).
- **Operator** — a person who wore the camera while working (every operator with footage is counted).
- **Hours** — measured on delivered clip duration; shares are computed over hours.

## Files

- `index.html` — the page, with the data inlined.
- `stats.json` — the same data as JSON: one block per component (`combined`, `stereo`, `multicam`) with hours, clip counts, unique
  counts, and hours by category, environment type, scene type, task category, category × scene and the top 300 scene × task pairs.
