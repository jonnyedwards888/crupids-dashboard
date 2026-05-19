# Quick Start Guide

## 🚀 Getting Started

1. **Start the development server:**
   ```bash
   npm run dev
   ```
   Then visit: http://localhost:5173/dashboard.html

2. **First time setup:**
   - Click the title "My Dashboard" to rename it to "Lucas's Dashboard" (or whatever you want)
   - Click the 👤 icon in the top right to upload your profile picture
   - Click the ⚙️ icon to set your wake/sleep times

3. **Start your day:**
   - Click the center circle (the progress ring) to start tracking your day
   - This initializes the day timer

## 📝 Working with Tasks

### Adding Tasks
- Type in the input box at the bottom of each card
- Click "+ Add" to add normally
- Click "✨ Polish" to use AI (requires Anthropic API key)

### Setting Priorities
1. Find the colored dot to the left of each task (between the drag handle and checkbox)
2. Click the dot
3. Choose your priority:
   - 🔴 Red = High priority (urgent)
   - 🟠 Orange = Medium priority  
   - 🟢 Green = Low priority
   - ⚪ White = No priority

### Moving Tasks
- **Reorder:** Drag the ⋮⋮ handle up/down within the same list
- **Push to tomorrow:** Drag any task from Today down to the "Plan tomorrow" card
  - The card will highlight yellow when you can drop
- **Bulk push:** Click "Push remaining to tomorrow →" button

### Completing Tasks
- Check the box to mark complete
- Completed tasks contribute to your streak
- Complete ALL tasks in a day to maintain your streak

## ⚙️ Settings & Stats

Click the ⚙️ icon to see:

### Settings
- **Wake time:** When your day starts (default 8 AM)
- **Sleep time:** When your day ends (default 12 AM / midnight)

### Statistics
- **Total tasks completed:** Lifetime count
- **Current streak:** Days in a row with all tasks done
- **Days tracked:** How many days you've used the dashboard
- **Best streak:** Your longest streak ever

## 🎯 The Goal Ticker

The scrolling banner at the top cycles through:
- Your incomplete tasks (when you have tasks)
- "All done" message (when everything is checked)
- "No goals" message (when list is empty)

Updates automatically when you add/complete tasks.

## 📊 The Day Ring

The center circle shows:
- **Percentage:** How far through your awake time
- **Phase:** Morning, Midday, Afternoon, Evening, Bedtime
- **Color:** Changes from yellow → orange → red → purple as day progresses
- **Time remaining:** Hours/minutes left in your awake window

**Before you start:** Shows "READY" - click to begin
**After you start:** Live tracking of your day

## 🔄 Automatic Features

### Daily Rollover
At 6 AM each day:
- Incomplete tasks from yesterday move to today
- New "Tomorrow" section unlocks
- Yesterday's completed tasks are archived

### Streak Calculation
- Complete all tasks = streak +1
- Leave any incomplete = streak resets to 0
- Best streak is saved forever

### Data Persistence
Everything saves automatically:
- Tasks and priorities
- Completion status
- Profile picture
- Custom title
- Settings
- Streak data
- Daily start times

No save button needed - just use the dashboard!

## 🎨 UI Tips

### Hover Effects
- Profile picture: Scales up slightly
- Settings button: Border brightens
- Tasks: Shows drag handle and delete button
- Buttons: Lift effect on hover

### Keyboard Shortcuts
- **Enter** in any input field: Adds the task
- **Enter** while editing title: Saves
- **Escape** while editing title: Cancels
- **Click outside** priority selector: Closes it

### Visual Feedback
- Drag over tomorrow card: Yellow outline
- Drag between tasks: Blue line shows drop position
- Queue button active: Yellow glow
- Completed task: Faded with strikethrough
- All done: Green glow on progress card

## 🚢 Deploy to Netlify

1. Push your code to GitHub
2. Connect repository to Netlify
3. Configure:
   - **Build command:** `npm run build`
   - **Publish directory:** `dist`
4. Deploy!

The `netlify.toml` file handles the rest (routing, build config, etc.)

## 💡 Pro Tips

1. **Start small:** Don't add 20 tasks on day one. Start with 3-5 achievable goals.

2. **Use priorities:** Not everything is urgent. Most tasks should be green or orange.

3. **Plan tonight:** Add tomorrow's tasks before bed while they're fresh in your mind.

4. **Drag to defer:** If something can wait, drag it to tomorrow instead of leaving it incomplete.

5. **Maintain streaks:** They're motivating! But don't stress if you break one - just start again.

6. **Adjust wake/sleep:** Match your actual schedule. Night owl? Set wake=12, sleep=4 (next day).

7. **Click to start:** Start your day when you're actually ready to work, not automatically.

## 🐛 Troubleshooting

**Tasks disappeared?**
- They rolled over to today automatically (check the date under "Today")

**Can't drag to tomorrow?**
- Make sure you're dragging from Today list (can't drag tomorrow→today)
- Yellow highlight shows valid drop zone

**Ring not updating?**
- Click the ring to start your day
- Check settings for correct wake/sleep times

**Changes not saving?**
- They are! localStorage auto-saves everything
- Try refreshing - your data will still be there

**Priority selector stuck?**
- Click anywhere outside it to close
- Or click the dot again

## 📱 Mobile Use

The dashboard works on mobile, but desktop is recommended for:
- Drag and drop (harder on touch)
- Comfortable typing
- Better visibility of all sections

Mobile still works for:
- Checking tasks
- Viewing progress
- Adding quick tasks

---

Enjoy your new dashboard! 🎉
