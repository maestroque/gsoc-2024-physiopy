> [!NOTE]  
> **Dates:** 27/5 - 31/5  
> **Intensity:** Low  
> **Primary Goal**: Define peakdet and phys2denoise interoperability

# Plans
- Find a proper structure for common interfacing of peakdet and phys2denoise
- Should they be migrated to one package? Should one be a dependency of the other?
- Find ways to incorporate the `Physio` class in `phys2denoise`
- Discuss what directions could be taken off from https://github.com/physiopy/peakdet/pull/61

### Pending from Previous Weeks
- Finalize Loguru https://github.com/physiopy/peakdet/pull/62
- Add pre-commit to peakdet https://github.com/physiopy/peakdet/pull/67
### New Tasks

### Misc
- Workflow Sessions
	- [[Mary Workflow Session]]
	- [[Marie-Eve Workflow Session]]
	- [[Stefano Workflow Session]]
- Timeline Finalization

# Meeting Agenda
- Dev
	- pre-commit PR
		- Fix the unit tests in a PR
		- pre-commit PR is ready but unit tests are currently failing
		- docs error
		- Once pre-commit passes
- Physio Object
	- Mary and Marie-Eve think that we should use physio-utils and migrate the Physio object
	- Stef: Have both function oriented and object oriented in phys2denoise
	- The object that tracks every step is really powerful

	- Mary: What if we moved more things to phys-utils and then even rename the peakdet package.
	- How are we going to be different from https://github.com/CoAxLab/niphlem ? 
	- **Actions**: Trying out phys-utils and migrating the physio object
- Logging
	- What was the idea for Gooey in peakdet -> Removing it
- Extra features (were not discussed in this meeting)
	- Masking untrusted data
	- Automatic detection of windows of interest in visual inspection
	- Peak Interpolation of double troughs
	- NK integration for filtering options
	- Use of json files for configurations
	- BIDS input/output compatibility
	- Extracting info automatically from json files in BIDS
	- Interpolating peaks
---
# Week sum-up
- All Loguru integration actions on peakdet are addressed and PR is ready to merge
- `pre-commit` addition PR is also ready to merge
- Workflow sessions were insightful. Many interesting features based on user experience were discussed, to be determined in the following weeks after the `phys2denoise`/`peakdet` restructuring 

# Actions
- Finalize Loguru PR on `phys2denoise` as well (not urgent)
- Migrate Physio object in `phys-utils`

# Remarks