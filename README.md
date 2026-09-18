# Tool Pocket Generator V108

## Provenance
Built directly from the immediately preceding V107 FINAL build ZIP. No reconstruction or patch source was used.

## Change
Fixed the STL export geometry-check gate so a current geometry check is actually executed when the stored check signature is stale, instead of the JavaScript short-circuit preventing `check()` from running. Once the current geometry check passes, the existing STL export path proceeds unchanged.

## FR STL
The V107 FR STL implementation is retained unchanged. No FR geometry algorithm was changed.

## Not changed
Detect exact tool outline, physical-grid calibration, measurements, editing, Close Profile, JSON export/import, workspace behaviour, FR placement, and STL geometry construction were not intentionally changed.

## Verification
- V107 FINAL used as direct source: PASS
- Export STL gate corrected: PASS
- FR STL construction retained: PASS
- JavaScript syntax check: PASS
- ZIP integrity: PASS
- Exactly 4 files in ZIP: PASS
- Exactly 1 README: PASS
