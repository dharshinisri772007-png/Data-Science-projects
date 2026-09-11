import pandas as pd
df=pd.read_csv("DMart.csv")
display(df)

import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd


# 1. DATA


months = ["Jan", "Feb", "Mar", "Apr", "May", "Jun"]
sales = [20, 35, 50, 45, 70, 85]


# 2. PLOT CUSTOMIZATION
# Titles, Labels, Colors


plt.style.use("seaborn-v0_8-whitegrid")

plt.figure(figsize=(10, 6))

plt.plot(
    months,
    sales,
    color="blue",
    linewidth=3,
    linestyle="-",
    marker="*",
    markersize=9,
    markerfacecolor="green",
    markeredgecolor="white",
    markeredgewidth=1.5,
    label="Monthly Sales"
)

# Title
plt.title(
    "Monthly Sales Analysis",
    fontsize=20,
    fontweight="bold",
    color="darkblue",
    pad=20
)

# Labels
plt.xlabel(
    "Month",
    fontsize=14,
    fontweight="bold",
    color="darkgreen"
)

plt.ylabel(
    "Sales",
    fontsize=14,
    fontweight="bold",
    color="darkred"
)



# 3. GRIDS AND STYLES


plt.grid(
    True,
    linestyle="--",
    linewidth=0.8,
    alpha=0.6
)

# Tick customization
plt.xticks(fontsize=12)
plt.yticks(fontsize=12)



# 4. THEMES AND SPACING


# Chart background
plt.gca().set_facecolor("#F5F9FF")

# Remove top and right borders
plt.gca().spines["top"].set_visible(False)
plt.gca().spines["right"].set_visible(False)

# Legend
plt.legend(
    loc="upper left",
    fontsize=12,
    shadow=True
)

# Add values
for x, y in zip(months, sales):
    plt.text(
        x,
        y + 2,
        str(y),
        ha="center",
        fontsize=11,
        fontweight="bold"
    )

# Spacing
plt.tight_layout()

plt.show()



# 5. ADVANCED PLOT - HEATMAP


data = {
    "Maths": [80, 70, 90, 60, 85],
    "Python": [85, 75, 95, 65, 90],
    "Statistics": [78, 72, 88, 70, 82]
}

df = pd.DataFrame(data)

plt.figure(figsize=(8, 5))

sns.heatmap(
    df,
    annot=True,
    cmap="YlGnBu",
    linewidths=1
)

plt.title(
    "Student Marks Heatmap",
    fontsize=18,
    fontweight="bold"
)

plt.xlabel("Subjects")
plt.ylabel("Students")

plt.tight_layout()

plt.show()


# 6. PAIRPLOT
# Multivariate Visualization


data = {
    "Age": [20, 21, 22, 23, 24, 25],
    "Study_Hours": [2, 3, 5, 6, 7, 8],
    "Marks": [50, 55, 65, 70, 80, 90]
}

df = pd.DataFrame(data)

sns.pairplot(df)

plt.show()
