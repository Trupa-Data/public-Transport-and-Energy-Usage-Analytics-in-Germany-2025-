Public Transport & Energy Usage Analytics in Germany (2025)

Wanted to check if there's real link between how much people use public transport in German cities and how much energy those cities burn through. pulled some open government data and dug in with python.


The Idea

Looked at ten cities — Berlin, Munich, Hamburg, Frankfurt, Stuttgart, Cologne, Düsseldorf, Leipzig, Dresden, Bremen. Cleaned up the ridership and energy numbers in Pandas, then plotted them together to see if the two actually move with each other or if it was just a hunch.

Turns out they do, pretty closely.

What I Notice

Berlin's numbers are honestly kind of wild compared to the rest — over 4 million riders a day, way ahead of Munich and Hamburg which come next. After Frankfurt there's a big drop into the mid-sized cities and things flatten out from there.

The energy line follows almost the same shape as ridership, city by city. Makes sense when you think about it — more trains running, more stations, more power needed — but it was still nice actually seeing it hold up across all ten instead of just the big three.

Couple other things:
- Energy use spikes around the usual morning/evening rush windows
- Mid-sized cities like Stuttgart and Cologne have flatter, more predictable energy use than the big ones — probably easier to plan around
- Ridership drops a lot on weekends but energy consumption barely moves, so a good chunk of that energy isn't really tied to how many people show up. Just infrastructure sitting there running.

Tools

Python — Pandas for cleaning, Matplotlib/Seaborn for the charts. Data's from Germany's open transport and energy portals.

Folder Layouts


├── data/
├── notebooks/
├── scripts/
├── visuals/
└── README.md


Running it

Clone it, install the requirements, go through the notebooks in order — cleaning first, then the analysis and charts.

Data's from 2025 releases, so numbers might look a bit different if you check against something more recent.
<img width="2048" height="1024" alt="image" src="https://github.com/user-attachments/assets/fe3b156a-5741-493d-a1c7-17abd0e780ba" />
