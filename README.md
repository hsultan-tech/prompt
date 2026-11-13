Use the frontend-design skill to refine the existing Kairos Goal Journey interface.

The current implementation is much better than before. The light theme, 3D models, and goal-specific content are working. DO NOT redesign the experience from scratch.

I am providing screenshots showing Owen Patel's anniversary trip to Japan, the 3D suitcase, and the expanded planning controls.

Focus on three specific improvements.

### 1. Redesign the left information panel

The left column currently feels like several disconnected text elements. The content hierarchy is weak, and some financial information gets pushed toward the bottom timeline.

Create a refined editorial composition:

- Small client and goal-category label.
- Large, beautiful goal headline.
- One short supporting description.
- Clearly emphasized target amount and target date.
- Two supporting financial metrics: projected amount and shortfall/surplus.
- One elegant status or financial insight section.
- One prominent "Explore the Plan" action.

Make the typography deliberate and consistent.

Keep the headline expressive but avoid excessively large text that causes clipping or pushes financial metrics below the viewport.

Remove redundant explanatory text and decorative elements.

The entire initial hero should remain visible at 1440×900 without colliding with the bottom milestone navigation.

### 2. Make all 3D goal objects larger and better framed

The suitcase currently looks too small relative to the large empty right-hand stage.

Increase its apparent size by approximately 50–80%, subject to fitting the entire object within the available canvas.

Do this through proper Three.js model bounds, camera distance, field of view and scene framing, NOT by blindly scaling the CSS canvas.

For each 3D asset:
- Calculate or inspect its bounding box.
- Center the model appropriately.
- Frame the object based on its dimensions.
- Maintain a comfortable margin around its silhouette.
- Keep the camera angle attractive and intentional.
- Retain beautiful lighting and material detail.
- Introduce a soft, believable grounding shadow.
- Use subtle floating or idle motion where appropriate.

Different shapes need different framing. A suitcase, car, house or graduation cap should not all use identical camera settings.

Create per-asset framing configuration where necessary.

Do not break the existing car model, asset registry or goal selection transitions.

### 3. Redesign the expanded financial planning experience

Currently, clicking Explore the Plan causes the chart and scenario sliders to appear in a narrow left column, making the page feel unbalanced and unfinished.

Do not simply stack these controls below the hero headline.

Instead, create a coordinated expanded planning mode:

- Preserve the beautiful 3D scene.
- Transition the layout smoothly to provide more room for financial analysis.
- Give the projection chart enough width to be easily understood.
- Group scenario sliders inside an organized planning section.
- Clearly show current trajectory, target, projected shortfall and adjusted outcome.
- Maintain a visible way to return to the clean cinematic hero.
- Prevent content from overlapping the bottom goal navigation.

The financial analysis should feel like a thoughtfully designed planning workspace, not a form inserted into a narrow sidebar.

### 4. Visual standards

Preserve the existing Kairos light theme and restrained Scotiabank red accents.

Target a premium, refined institutional aesthetic with the presentation quality of a high-end interactive website.

Use:
- Strong typographic hierarchy
- Excellent alignment
- Intentional negative space
- Restrained, coordinated motion
- Clean financial information
- Large, recognizable 3D objects

Avoid:
- Generic dashboard cards
- Unnecessary gradients
- Excessive badges
- Tiny 3D objects
- Giant empty areas
- Clipped or overlapping content
- New unrelated features

### 5. Preserve functionality

Do not break:
- Client-specific milestones
- Add Goal
- Existing 3D models
- Financial projection calculations
- Scenario controls
- Client switching
- Homepage-to-client transitions
- Opportunity navigation

Do not change the underlying synthetic data or financial assumptions during this visual refinement.

### 6. Verify the rendered result

Inspect the current implementation before editing.

Render and review at 1440×900.

Capture both the initial hero and expanded planning state.

Verify the suitcase is substantially larger, the left column has a coherent hierarchy, the financial planning state is readable, and the timeline does not overlap any content.

Also test at least the car and house scenes to ensure the new camera-framing logic works for differently shaped models.

Run the existing build and lint checks.

Make the changes directly. Do not stop after producing a design proposal.

**The goal is to refine an already promising experience into a visually exceptional, cohesive product, not rebuild it.**
