# Mealie ingredient import walkthroughs

Review videos for [SparkyFitness PR #3396](https://github.com/CodeWithCJ/SparkyFitness/pull/3396), recorded against `f407fe860cd696af00a55f3e089f006a8df96f02`.

- [Web walkthrough (1:33)](mealie-ingredient-import-web.mp4)
- [Android emulator walkthrough (2:05)](mealie-ingredient-import-android.mp4)

These are recordings of the running clients using synthetic foods, a synthetic account and a local Mealie-compatible API fixture. Previously saved food mappings are reused; the web walkthrough also opens the ordinary food picker and quantity editor. Android runs current JavaScript in an existing development build. No private instance, real health data or physical device was used.

The example recipe contains 400 g dry rice and 800 g raw chicken, with four servings and an example finished batch weight of 1,800 g. Its total nutrition is 2,400 kcal: 450 g is 600 kcal, and 225 g is 300 kcal.

The web walkthrough changes the rice amount to 500 g for one preparation in the diary form. That 225 g portion is recalculated to 345 kcal. The reusable meal retains its original ingredients and nutrition. The Android diary shows both that separate preparation and the ordinary 225 g / 300 kcal portion. The additional portion adjustment is previewed and cancelled.

Only the explicit nutrition-sync action writes to the Mealie fixture. Saving the reusable meals and diary entries does not change its recipe ingredients or instructions.

The videos are edited walkthroughs: idle waits are removed, some typing is accelerated and brief reading pauses are added. They are not performance measurements. iOS and physical-device flows are not shown.
