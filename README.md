# 🚀 Exploring the McCall Job Search Model

👋 Welcome to this repository.

This project is a complete reconstruction and integration of the **McCall Job Search Model**, one of the most famous frameworks in labor economics.

I created this notebook (`mccall_search_dynamics.ipynb`) to deeply understand how dynamic programming applies to unemployment and wage decisions. Instead of having scattered scripts, I’ve unified everything into a single, cohesive story—from the simplest model to complex ones with continuous shocks.

I built this to learn, and I'm sharing it in hopes that it might spark some ideas for you!

## 🌟 What's Inside?

This isn't just code; it's a guided tour. The notebook builds up complexity step-by-step:

1.  **The Basics (Baseline Model)**: We start simple. A worker, a wage offer, and a choice. When should they say "yes"?
2.  **Reality Check (Separation)**: Jobs don't last forever. We add the risk of getting fired ($\alpha$) and see how that changes the math.
3.  **Sticky Wages (Markov Process)**: Good times and bad times often cluster together. We model wages that are correlated over time.
4.  **Going Continuous (Fitted VFI)**: Real wages aren't just discrete points. We use **Fitted Value Function Iteration** to handle continuous states—a crucial technique in modern macro.
5.  **Complex Shocks (Persistent vs. Transitory)**: We decompose wages into "luck" (transitory) and "skill/productivity" (persistent) to see how they affect the reservation wage differently.
6.  **Life of a Worker (Simulation)**: Finally, we simulate a single agent's life to visualize their career path, unemployment spells, and decisions in real-time.

## 🛠️ Under the Hood

I used **Python** and **JAX** for this project.
*   **Why JAX?** It allows for Just-In-Time (JIT) compilation, making our iterative solvers blazingly fast. ⚡
*   **Visualization**: Lots of plots using Matplotlib to build intuition.
*   **Math**: Every section starts with the economic theory and LaTeX equations, so you know exactly what we are coding.

## 🏃‍♂️ How to Run It

1.  **Clone the repo**:
    ```bash
    git clone https://github.com/yourusername/mccall-search-model.git
    cd mccall-search-model
    ```

2.  **Get the tools** (you'll need JAX and QuantEcon):
    ```bash
    pip install jax jaxlib matplotlib numpy quantecon
    ```

3.  **Dive in**:
    ```bash
    jupyter notebook mccall_search_dynamics.ipynb
    ```
    Run it from top to bottom. It’s self-contained!

## 📚 References

This work stands on the shoulders of giants. It is based on the excellent lecture series by [QuantEcon](https://quantecon.org/). I've rewritten and reorganized the code to fit my own learning structure and to utilize JAX features more explicitly.

## 🙏 Special Thanks

A huge thank you to **Professor John Stachurski** for his amazing teaching. His guidance on computational economics opened my eyes to these tools and inspired me to build this project. Thank you for showing us the way! 🚀

---

*Happy Coding & Searching!* 🕵️‍♂️💼
