STOP adding features. The current Financial Goal Journey implementation is visually unacceptable.

Look at the rendered screenshot and critically evaluate what you produced.

The intended experience was a cinematic, award-quality 3D financial goal presentation. Instead, the page is a nearly empty dark rectangle with cramped financial text, an almost invisible car, and a basic row of timeline dots.

This is not remotely close to the supplied visual references.

**YOUR ONLY TASK RIGHT NOW IS TO COMPLETELY FIX THE HERO EXPERIENCE.**

### 1. Diagnose the invisible 3D model

The 3D car is practically invisible.

Inspect the actual React Three Fiber scene, GLB asset, camera, lighting, materials, canvas sizing, and CSS stacking.

Determine whether:
- The model is loading correctly.
- The camera is pointing at the model and framing its complete bounds.
- The model scale and position are correct.
- Materials are receiving sufficient lighting.
- CSS overlays or parent opacity are hiding the canvas.
- The scene is clipped or rendered behind another element.

Fix the root cause rather than blindly increasing brightness or adding CSS effects.

The car must be clearly recognizable, rendered at a substantial size, and beautifully illuminated.

### 2. Completely rethink the hero composition

Use a sophisticated two-column editorial composition.

LEFT: approximately 35–40% of the hero.
- Beautiful large serif or editorial headline.
- Client and goal context.
- Target amount and date.
- Projected outcome and shortfall.
- One obvious primary action.

RIGHT: approximately 60–65% of the hero.
- A large, high-quality 3D car.
- Three-quarter perspective.
- Cinematic studio lighting.
- Soft shadows and subtle atmospheric depth.
- Clean graphite environment.
- No overlapping text.
- No meaningless empty space.

The car must be the dominant visual element.

Do not use a flat image as a substitute for the 3D model.

### 3. Improve the entire visual direction

The current dark textured background looks muddy and cheap.

Replace it with a deliberate, restrained, premium studio environment.

Take inspiration from sophisticated automotive product experiences and award-winning interactive websites.

Use:
- Exceptional typography.
- Carefully balanced negative space.
- Strong contrast and legibility.
- Subtle Scotiabank red as a restrained accent.
- Beautiful studio lighting.
- Intentional animation.

Avoid generic dashboards, excessive gradients, decorative floating particles, stock UI cards, and random glow effects.

### 4. Preserve the functional work

Keep the existing:
- Financial projection calculations.
- Goal selection functionality.
- Scenario planning functionality.
- Client navigation.
- Existing routes.

Do not build more goals or product recommendations during this iteration.

### 5. Fix date accuracy

The screenshot says October 2028 is 24 months away from November 2026.

Use one consistent demo as-of date. Make the goal horizon and projection calculations agree with that date.

### 6. Verify visually, not just technically

Run the app and inspect the ACTUAL rendered result at 1440×900.

Do not consider the task complete simply because the build succeeds.

Verify:
- The complete car is clearly visible.
- The car occupies a meaningful portion of the right side.
- The lighting and materials look premium.
- Financial numbers are immediately readable.
- The composition feels balanced.
- No element is clipped or overlapping.

Capture a screenshot if browser tooling is available. If not, explicitly tell me visual verification was not possible.

Compare the implementation against the references and fix the obvious weaknesses.

Do not add any more features until this first screen looks genuinely excellent.

I want a beautifully designed interactive 3D product experience, NOT a conventional financial dashboard with a 3D model hidden somewhere in the background.
