# COMPASS Interview Tools

**Critical Operations Mapping & Process Analysis System**

A web-based interview system for extracting business process structures using Universal Process Grammar (UPG) methodology.

---

## 🚀 Quick Start

### For Lisa (or other team members):

**USE THIS FILE:** `compass_unified_web_v2.html` ⭐

This is the **fixed and tested** version with Stage 2 bug corrections.

### How to Run:

1. **Download** `compass_unified_web_v2.html` to your local machine
2. **Open** the file in your web browser (Chrome, Firefox, Edge)
3. **Enter** your Anthropic API key when prompted
4. **Choose** Stage 1 or Stage 2:
   - **Stage 1**: Structural Interview (Pathways → Milestones → Jobs)
   - **Stage 2**: Task Interview (Jobs → Tasks → Steps)

---

## 📋 Two-Stage Process

### Stage 1: Structural Interview
**Purpose:** Define high-level process structure

**Extracts:**
- Pathway definition
- Milestones (major phases)
- Jobs (work packages within milestones)
- Actors (who performs the work)
- Duration estimates

**Output:** JSON file with hierarchical structure

**Time:** 15-30 minutes depending on process complexity

---

### Stage 2: Task Interview
**Purpose:** Extract detailed task and step-level information

**Requires:** Stage 1 JSON output file

**Extracts:**
- Tasks within each Job
- Steps in Action-Object-Conditional format
- Actor assignments
- Duration estimates
- Action/Object libraries

**Output:** JSON file with complete task details

**Time:** 5-10 minutes per Job

---

## 🐛 Known Issues & Fixes

### v2.html Fixes (January 13, 2026):
- ✅ **Stage 2 hanging bug fixed** - Jobs now properly handled as strings (not objects)
- ✅ **Enhanced UPG Task prompts** - Full structure requirements included
- ✅ **Increased API timeout** - 90 seconds for Stage 2 interviews
- ✅ **Task extraction improvements** - Action-Object-Conditional parsing
- ✅ **Intelligence protocols** - Redundancy detection, exception handling

### v1.0.html Issues:
- ❌ Stage 2 would hang on "Loading 0/23 Jobs"
- ❌ Line 880 bug: accessed `.name` on job strings
- ❌ Minimal Stage 2 system prompts

**Recommendation:** Always use v2.html

---

## 📁 File Inventory

| File | Status | Purpose |
|------|--------|---------|
| **compass_unified_web_v2.html** | ✅ **USE THIS** | Fixed Stage 2 with all bug corrections |
| COMPASS_Complete_v1.0.html | 🔒 Reference only | Original version (has Stage 2 bugs) |
| index.html | Web landing | Project landing page |
| logo-white.png | Asset | COMPASS logo |

---

## 🧪 Testing Checklist for Lisa

**Stage 1 Test:**
1. Open `compass_unified_web_v2.html`
2. Enter API key
3. Click "Stage 1" card
4. Enter process name (e.g., "Test Process")
5. Begin interview
6. Answer 5-10 questions
7. Export JSON when complete

**Stage 2 Test:**
1. Open `compass_unified_web_v2.html` (fresh page)
2. Enter API key
3. Click "Stage 2" card
4. Upload your Stage 1 JSON file (e.g., `COMPASS_Onboarding_homeless_veterans_onto_(MHBG).json`)
5. Click "Begin Task Interviews"
6. Should see first job interview start (not hang!)
7. Complete interview for 1-2 jobs
8. Export Stage 2 JSON when done

---

## 💡 Tips

**For Best Results:**
- Use specific, concrete examples when answering questions
- Mention edge cases and exceptions when asked
- Provide duration estimates (e.g., "2-3 hours" not just "a while")
- Be consistent with actor names
- Answer one question at a time - don't combine multiple answers

**If Something Goes Wrong:**
- Check browser console (F12) for error messages
- Verify API key is correct
- Ensure Stage 1 JSON is properly formatted
- Try refreshing the page and starting over

---

## 📞 Support

**Questions?** Contact:
- Pat Boulay - Co-Founder & Chief Architect, xFormative AI
- p.boulay@xformative.ai

**Project Info:**
- Website: https://xformative.ai
- Patent: Provisional Application #63/954,078
- Technology: Universal Process Grammar (UPG) methodology
- Based on: 1997-1999 MAP framework (Prudential deployment)

---

## 📜 Version History

**v2.0 (January 13, 2026)**
- Fixed Stage 2 job loading bug (line 880)
- Enhanced UPG Task extraction prompts
- Increased API timeouts for complex interviews
- Added Action-Object-Conditional step parsing
- Implemented intelligence protocols

**v1.0 (January 2026)**
- Initial two-stage interview system
- Stage 1 structural extraction working
- Stage 2 had hanging issues (now fixed in v2)

---

**Last Updated:** January 15, 2026

