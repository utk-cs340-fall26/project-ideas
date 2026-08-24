# Meal Map - A Recipe & Meal Planning App

Cooking at home shouldn't require a spreadsheet's worth of planning. Between decision paralysis, scattered recipe sources, and the tedium of building a grocery list from scratch, many people default to takeout or the same five meals on repeat. This app aims to make home cooking feel effortless by combining recipe management, meal planning, and grocery list generation in one place — built natively for iPhone, iPad, and Mac so it fits into however someone actually plans their week.

On launch, users see their favorited and most-used recipes first, with calories/macros visible at a glance. A search bar covers recipe names, ingredients, and cook time, and every recipe supports 1-5 star ratings plus a notes field for personal tweaks. From any recipe, users can generate a grocery list with one tap and export it to Reminders, Notes, or any app via the native share sheet.

## Core Features

Create/edit/delete recipes with ingredients, quantities, instructions, and prep/cook time
Categories and custom tags (vegetarian, quick, low-prep, etc.)
Search, favorites, ratings, and personal notes per recipe
Persistent local storage

## Advanced Features

Weekly meal planner with calendar view
Automatic grocery list generation and export
Nutrition breakdown per recipe
Recipe importing from any recipe website via URL
iCloud sync across all devices

## Technologies

Swift + SwiftUI, targeting a single multiplatform codebase for iOS, iPadOS, and macOS
SwiftData for persistence, with CloudKit for cross-device sync
Spoonacular API (with USDA FoodData Central as a nutrition fallback) for recipe search and nutrition data
Schema.org/Recipe JSON-LD parsing for importing recipes from external websites
EventKit and SwiftUI's ShareLink for exporting grocery lists to Reminders or other apps
SF Symbols and native SwiftUI animations for a clean, polished interface

## Intended Users

Anyone who cooks regularly but finds planning tedious — busy professionals who want to meal-prep without the mental overhead, families juggling different dietary needs and tastes, and home cooks who collect recipes from a dozen different sources and want them all in one searchable place. Because the app runs natively across iPhone, iPad, and Mac with shared data, it fits naturally into how people already move between devices — jotting a recipe idea on a phone, planning the week on an iPad, and pulling up instructions on a Mac while cooking.
