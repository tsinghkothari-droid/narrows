# Narrows

Narrows is a one-page tool that animates a process-flow analysis. You describe a process in a few numbers. Narrows draws it as a channel and shows which step limits the whole process.

The animation has eight beats:

1. Flow unit
2. Process map
3. Capacity of each step
4. Bottleneck against demand
5. Utilization
6. Little's Law (I = R × T)
7. The fix
8. Whole-process effect, before and after

## Open it

Double-click `index.html`. It opens in any modern browser.

There is no build step and no server. The page loads its fonts from Google Fonts, so the type looks best when you are online. Everything else works offline.

## Controls

- **Play / Pause** runs the eight beats in order.
- **Back / Next**, or the ← → keys, move one beat.
- Click a beat on the rail, or press 1–8, to jump.
- Add `#4` to the address to open on beat 4.

## Edit the brief

Use the **Your process** panel. The drawing and the maths recompute as you type.

| Field | What to enter |
| --- | --- |
| Process, workplace | Names for the title block |
| You count one… / …and many | The flow unit, for example `order` / `orders` |
| It starts when / It ends when | The two events that bound the process |
| Demand | Units that arrive per hour at the busy time |
| Steps | Name, resource, how many resources, minutes per unit |
| The fix to test | A step and its new resource count |
| The tempting alternative | Optional. A second change to compare |
| Money | Optional. Margin per unit, busy hours a day, cost of the fix |

The page saves your brief in the browser on your device. **Load kitchen example** restores the demo. **Start blank** clears the form.

## The formulas

- Capacity = resources ÷ time per unit (× 60 for units per hour)
- Process capacity = the smallest step capacity
- Flow rate R = the smaller of demand and process capacity
- Utilization = flow rate ÷ capacity
- Little's Law: I = R × T (units in process = flow rate × flow time)

The model assumes that steps run one after the other, each resource handles one unit at a time, step times are fixed, and work arrives evenly.

## About the demo

The default data is a worked example: a small delivery kitchen at rush hour. The kitchen and all its figures are fictional. Replace them with a process from your own workplace.

In the example, demand is 24 orders/h and the steamer can finish only 20/h. A third cook does not help, because the steamer still sets the pace. A second steamer lifts capacity to 30/h, and demand becomes the limit at 24/h.
