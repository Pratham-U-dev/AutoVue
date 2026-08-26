## Research Gaps the Paper Identifies — Directly Applicable to You

The paper explicitly calls out these gaps, and your project currently has all of them:

* Gap 1 — No real-time feedback loop. The paper says most eco-driving systems don't provide context-aware feedback during operation. Your dashboard shows graphs, but it doesn't tell the driver anything actionable in real time.

* Gap 2 — No fuel efficiency prediction. This is listed as a roadmap item for you and is one of the paper's core domains. Random Forest or LSTM on your existing 10 sensor fields can estimate fuel consumption per second (FCR).

* Gap 3 — No anomaly detection. This is in your roadmap but not built. The paper's Table 9 shows TEDA-RLS achieves real-time outlier detection at 243 µs/cycle — fast enough for embedded use.

* Gap 4 — No composite vehicle health score. The paper mentions this pattern: instead of a binary Normal/Warning, a 0–100 weighted score based on multiple sensor conditions is more useful to stakeholders.

* Gap 5 — KMeans gives no interpretable features to the user. The paper highlights that behavioral feature extraction (hard braking events, sharp turns, idling percentage) is what makes behavior profiling useful. Your current model gives cluster_id: 0 with no explanation.
