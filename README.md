import matplotlib.pyplot as plt
import matplotlib.patches as patches
from matplotlib.patheffects import withStroke

# Function to apply text shadow
def shadow_text(ax, x, y, text, fontsize, color, shadow_color, **kwargs):
    shadow_effect = withStroke(linewidth=3, foreground=shadow_color, alpha=0.6)
    ax.text(x, y, text, fontsize=fontsize, color=color, path_effects=[shadow_effect], **kwargs)

# Create a figure and axis
fig, ax = plt.subplots(figsize=(12, 6))
ax.set_xlim(0, 12)
ax.set_ylim(0, 6)
ax.axis('off')

# Background gradient
for i in range(100):
    ax.add_patch(
        patches.Rectangle(
            (0, i * 0.06), 12, 0.06,
            color=plt.cm.Blues(i / 100),
            lw=0
        )
    )

# Add main text
shadow_text(
    ax, 1, 4.5,
    "Hi there! I'm [Your Name]",
    fontsize=30, color='white', shadow_color='black', fontweight='bold'
)
shadow_text(
    ax, 1, 3.5,
    "Senior @ University of Pennsylvania",
    fontsize=20, color='white', shadow_color='black', fontweight='medium'
)

# Add bullets for key points
key_points = [
    "Accelerated Master's in Bioengineering",
    "Research in TBI, epilepsy, and image segmentation",
    "Founder of Our Beautiful Earth",
    "Passionate about mental health & climate impacts"
]

for i, point in enumerate(key_points):
    shadow_text(
        ax, 1.5, 3 - i * 0.5,
        f"- {point}",
        fontsize=18, color='white', shadow_color='black'
    )

# Footer
shadow_text(
    ax, 1, 0.5,
    "Connect with me: sheelp@sas.upenn.edu",
    fontsize=15, color='white', shadow_color='black'
)

# Save the graphic
plt.savefig("github_profile_graphic.png", dpi=300, bbox_inches='tight')
plt.show()

