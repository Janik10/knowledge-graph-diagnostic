# How many questions does a knowledge-graph diagnostic need, and what does one slip cost?

A small simulation of adaptive placement on a prerequisite graph: 150 synthetic topics in 10 layers, where a student's knowledge is downward closed (knowing a topic implies knowing its prerequisites).

**Key results (this simulation)**
- Choosing questions by bisection and inferring along the graph places a student in about **38 questions instead of 150**.
- With realistic noise (10% slip, 10% guess), one wrong answer on a high-leverage topic can mislabel a whole branch: accuracy drops to about 94%.
- Re-asking only **high-stakes** questions (those whose answer would decide many other topics) cuts misclassified topics **roughly in half (5.7% → 3.0%) for about 11 extra questions**, versus about 46 extra questions to re-ask everything.

**Caveats:** synthetic graph and a simple slip/guess model. The stronger version is soft inference: a probability per topic, with evidence propagated by weight instead of hard labels.

→ [Open the notebook](diagnostic_slip_analysis.ipynb)

By Jahangir Mammadli · [mammadli.dev](https://mammadli.dev)
