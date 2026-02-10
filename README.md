# Shawn Kemp Card Collection - Netlify Deployment

This folder contains everything you need to deploy your card collection website to Netlify.

## Files Included:

1. **index.html** - Your main website with all 644 cards
2. **cards-data.json** - Your complete card collection data with WordPress image URLs

## Deployment Steps:

### Step 1: Upload to Netlify
1. Drag the entire **shawn-kemp-site** folder to Netlify
2. Wait ~30 seconds for deployment
3. Done! Your site is live! 🎉

That's it! No API tokens, no environment variables, no downloads needed.

## How It Works:

- All your card data is stored in the `cards-data.json` file
- Images load directly from your WordPress site at reignmancollection.wordpress.com
- The website automatically constructs image URLs based on card names
- Example: "1991-92 Fleer #231 Shawn Kemp SD" → `1991-92-fleer-231-shawn-kemp-sd.jpg`

## Image URL Pattern:

Front images: `https://reignmancollection.wordpress.com/wp-content/uploads/[card-name].jpg`
Back images: `https://reignmancollection.wordpress.com/wp-content/uploads/[card-name]-back.jpg`

The card name is converted to lowercase with hyphens (spaces and special characters removed).

## If Some Images Don't Load:

Some cards might have slightly different naming on WordPress. You can:
1. Check the browser console to see which URLs are 404ing
2. Either rename files on WordPress to match the pattern
3. Or manually edit the `cards-data.json` file to match your actual WordPress filenames

## Updating Your Collection:

When you add new cards to Airtable:

1. Export your Airtable as CSV
2. Send me the new CSV file
3. I'll convert it to JSON with WordPress URLs
4. Replace the `cards-data.json` file
5. Drag the folder to Netlify again to update

**OR** if you're comfortable with JSON:
- You can manually edit the `cards-data.json` file to add/remove cards
- Just follow the same format as the existing entries

## Features:

✅ All 644 cards loaded instantly  
✅ Filter by Year, Brand, Set, Type  
✅ Search across all fields  
✅ Sort in multiple ways  
✅ Card flip animations on hover  
✅ Expandable details for each card  
✅ Comments section  
✅ Fully responsive design  
✅ Images load from your WordPress site (never expire!)

Enjoy your collection! 🏀
