Use the frontend-design skill. I need you to rescue the visual design of the existing Kairos Goal Journey.

**Your previous implementation is not visually acceptable. This task is not complete when the code builds. It is complete when the rendered application looks polished and works correctly.**

## FIRST: INSPECT THE ACTUAL APPLICATION

Before modifying code:

1. Find the existing Goal Journey route and its React components.
2. Start the development server using the project's existing scripts.
3. Use available VS Code browser tools, Playwright, or an existing browser automation integration to open the page at 1440×900.
4. Capture a screenshot and save it to `design-review/before.png`.
5. Visually inspect the rendered result if your tools support image inspection.
6. Inspect browser console messages and Three.js loading errors.

If browser tooling is unavailable, clearly report that limitation and use the source code and runtime diagnostics. Do not claim to have visually inspected a screenshot you cannot see.

## THE SPECIFIC PROBLEM

The existing screen looks like an unfinished dark dashboard.

The car is practically invisible. The text is crowded to the left, the right side is mostly empty, the background looks muddy, and the timeline is an unimpressive row of dots.

We need a deliberate design rebuild of the HERO, not another round of minor CSS changes.

## VISUAL TARGET

Create a premium cinematic automotive presentation integrated into a financial planning interface.

Target viewport: 1440×900.

Composition:

LEFT 35–40%:
- Client and goal identification.
- A striking editorial headline.
- Target amount and target date.
- Current savings and projected result.
- A prominent shortfall or surplus figure.
- One primary action: "Explore the Plan".

RIGHT 60–65%:
- A large, clearly visible REAL 3D car.
- Recognizable silhouette and premium materials.
- Three-quarter camera angle.
- High-quality studio lighting.
- Soft environmental shadows.
- Minimal atmospheric effects.
- No text overlapping the vehicle.

The vehicle should occupy approximately 65–80% of its available 3D canvas width and remain completely within the frame.

The 3D object must be instantly recognizable at normal viewing size.

Use a refined charcoal or dark graphite background, not a featureless black rectangle.

Typography should be expressive and confident. Use contrast, scale, and spacing to create hierarchy.

Scotiabank red should be a restrained accent, not a substitute for good composition.

## DEBUG THE 3D CAR PROPERLY

Before styling around the model, verify:

- GLB asset loads without errors.
- Canvas has correct dimensions.
- Camera position, lookAt target, near/far planes and field of view are correct.
- Model bounding box, scale and center are calculated.
- Camera framing accounts for the model's actual size.
- Materials are rendering correctly.
- Ambient, directional and environment lighting are sufficient.
- CSS stacking, opacity and clipping aren't hiding the model.

Temporarily use a bright neutral debugging environment to establish correct visibility.

Then reintroduce cinematic lighting.

Do not attempt to fix an invisible model using arbitrary CSS brightness, giant scaling values, or random camera adjustments.

If the asset itself is unsuitable, report that explicitly and use a better licensed asset rather than disguising the problem.

## FINANCIAL PRESENTATION

The financial information must remain extremely clear.

Show:
- Goal amount: $40,000.
- Current savings: $20,000.
- Monthly contribution: $600.
- Target horizon: 24 months.
- Projected savings derived from the existing calculation engine.
- Shortfall or surplus.
- Status: On Track or At Risk.

Use one consistent simulated as-of date for the 24-month horizon.

All figures must reconcile with the existing calculation engine. Do not fabricate numbers.

Do not add speculative AI success probabilities.

## TIMELINE DESIGN

For now, keep the goal navigation simple.

Use a refined horizontal goal selector anchored below the main composition.

It should visually support the hero, not compete with it.

Display readable labels and meaningful dates.

Do not build a new timeline system or additional goals during this pass.

## MOTION

Keep interactions deliberate and restrained.

- Subtle idle movement of the 3D car.
- Gentle pointer-driven rotation.
- Smooth text transitions.
- Refined entrance choreography.
- No aggressive camera movements, excessive zooming or bouncing.

Support reduced-motion preferences.

## NON-NEGOTIABLE CONSTRAINTS

Do not modify the existing homepage, client rail, opportunity pages, financial calculation engine, or unrelated components.

Preserve routing and navigation.

Do not implement new product recommendation features.

Do not add unnecessary dependencies.

## REQUIRED VISUAL VERIFICATION

After implementing:

1. Open the actual Goal Journey.
2. Capture `design-review/after.png` at 1440×900.
3. Verify that the car is visible and correctly framed.
4. Inspect the hero for clipping, excessive empty space, alignment issues and unreadable text.
5. Correct the largest visible problems.
6. Capture a final screenshot after corrections.
7. Run build and lint checks.

If visual inspection tools are available, complete at least two screenshot-based refinement passes.

Your final response must identify:
- The original cause of the poorly rendered car.
- What you changed.
- Which screenshots you generated.
- What was actually verified.
- Any remaining limitations.

Do not claim the result looks excellent without inspecting the rendered result.

**Success means the page looks like a carefully art-directed, interactive automotive product presentation that also communicates a clear financial planning decision.**

Do not add more features. Perfect this one screen first.
