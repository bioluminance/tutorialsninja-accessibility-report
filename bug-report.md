# 🐞 Accessibility Bug Report – TutorialsNinja Demo Store

**Test Date:** April 11, 2025  
**Audited By:** sivakandasamyv@gmail.com  
**Website:** [https://tutorialsninja.com/demo](https://tutorialsninja.com/demo)  
**Audit Tool Used:** Axe DevTools HTML (v4.103.6)  
**Standards Evaluated:** WCAG 2.1 AA  
**Total Issues Found:** 32  
- Critical: 9  
- Serious: 23  

---

## 🔴 Critical Issues (9) – Missing Accessible Names for Buttons

These buttons lack visible text, `aria-label`, or `aria-labelledby`. Screen readers cannot determine their function.

### 🔹 Rule Violated: `button-name`
- **WCAG 2.1 Reference:** 4.1.2 Name, Role, Value
- **Fix Recommendation:** Add `aria-label`, `title`, or descriptive text inside the button.

### 🧩 Affected Buttons:
1. Search button (magnifying glass icon only)
2. Wishlist button for "MacBook"
3. Wishlist button for "iPhone"
4. Wishlist button for "Apple Cinema"
5. Wishlist button for "Canon EOS 5D"
6. Compare button for "MacBook"
7. Compare button for "iPhone"
8. Compare button for "Apple Cinema"
9. Compare button for "Canon EOS 5D"

---

## 🟠 Serious Issues (23)

### ⚠️ Color Contrast Failures (21)

### 🔹 Rule Violated: `color-contrast`
- **WCAG 2.1 Reference:** 1.4.3 Contrast (Minimum)
- **Fix Recommendation:** Increase text color contrast to meet 4.5:1 ratio.

### 🧩 Affected Text Examples:
1. “My Account” link (grey on white)
2. “Wish List” link
3. “Shopping Cart” link
4. “Checkout” link
5. “Currency” button
6. “MacBook” product name
7. “iPhone” product name
8. “Apple Cinema” product name
9. “Canon EOS 5D” product name
10. Price: “Ex Tax: $500.00”
11. Price: “Ex Tax: $100.00”
12. Price: “Ex Tax: $80.00”
13. Price: “Ex Tax: $90.00”
14. Top navigation links
15. Featured product descriptions
16. Blue colored text links (`#23a1d1`)
17. Gray labels and badges
18. Product sorting dropdown
19. Product grid/filter info
20. Category listing text
21. Special price tags

---

### ⚠️ Other Serious Issues (2)

#### 🔹 Link Not Distinguishable by More Than Color
- **Rule Violated:** `link-in-text-block`
- **WCAG 2.1 Reference:** 1.4.1 Use of Color
- **Fix Recommendation:** Add underline or bold style to make links stand out.

**Example:** OpenCart link at the bottom of the page.

#### 🔹 Link Missing Accessible Name
- **Rule Violated:** `link-name`
- **WCAG 2.1 Reference:** 2.4.4 Link Purpose
- **Fix Recommendation:** Add `aria-label` to the icon-only link.

**Example:** Phone icon link (no screen reader-friendly label)

---

## ✅ Live Fix Test Results (DevTools Inspection)

After applying temporary HTML fixes using browser DevTools:
- Re-ran Axe scan → **Issue count reduced from 32 to 12**
- Shows that the issues can be resolved with small accessibility improvements (like adding labels and updating color styles)

---

## 📁 Related Files

- `tutorialsninja.com-2025-04-11.csv` – Raw CSV scan data
- `tutorialsninja.com-2025-04-11.json` – Raw JSON scan data
- This bug report: `bug-report.md`

---

## ✅ Summary

The TutorialsNinja Demo Store shows several key accessibility issues that can significantly affect users relying on assistive technology. Addressing these issues will improve compliance with WCAG 2.1 standards and enhance the experience for all users.

---

> Report Prepared By:  
> [sivakandasamyv@gmail.com]
> April 11, 2025  
