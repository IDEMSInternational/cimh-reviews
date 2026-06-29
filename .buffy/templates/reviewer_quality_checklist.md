## Data quality review checklist for @{{sender}}

*The author submitted stated their report type is {{report-type}}. Check that you have generated the right checklist.*

### Conflict of interest

- [ ] I confirm that I have no conflicts of interest (COIs) with reviewing this work by (@{{author}}), or that any perceived COIs have been waived by the editors for the purpose of this review.

### Code of conduct

- [ ] I confirm that I have read and will adhere to the [code of conduct](https://github.com/IDEMSInternational/cimh-reviews/blob/main/code_of_conduct.md).

### General checks

- [ ] **Repository:** Is the source code for this software available at {{repository}}?
- [ ] **PDF:** Is the pdf accessible and readable at {{pdf}}?

### Data quality report

- [ ] Report title is clearly stated including date of report preparation and author’s name
- [ ] Station details are provided including location information (province/district/longitude and latitude), period of record covered is specified, variables assessed are listed	
- [ ] Software and version used to produce QC outputs is stated e.g. R-Instat v0.8.14
- [ ] An inventory report has been produced and reviewed
- [ ] A summary of the QC checks performed is included - list which checks were run, not just which passed	
- [ ] Duplicates check
- [ ] Internal consistency checks between variables are reported where relevant e.g. tmax vs tmin, wet day vs rainfall amount
- [ ] Rainfall-specific quality checks
- [ ] Distribution of daily rainfall values is shown (e.g. histogram)	
- [ ] False zeros are investigated and reported	Days recorded as 0 mm surrounded by wet days; cross-check with neighbours if possible	
- [ ] Extreme daily values are listed and flagged for investigation i.e. values exceeding the station historical maximum should be noted	

### Temperature-specific quality checks

- [ ] Daily maximum temperature (`tmax`) distribution is shown e.g. box plots by month or season	
- [ ] Daily minimum temperature (`tmin`) distribution is shown
- [ ] Cases where `tmax` ≤ `tmin` are identified and listed. These are physically impossible and indicate recording or data entry errors	
- [ ] Cases where `tmax` – `tmin` < 2°C are identified. A very small diurnal range may indicate a transcription error	
- [ ] Outliers are identified using a clearly stated method e.g. ±3 standard deviations from monthly mean, or IQR-based. The outlier detection method is defined in the report. Flagged outliers are listed with dates and values		

### Presentation and readability

- [ ] All QC outputs (tables, plots) are labelled with titles, axis labels, and units		
- [ ] Flags and their meanings are defined in a legend or key		
- [ ] A summary of flagged records is included at the end of the report. Total counts by type and variable	
- [ ] The report follows the standard ZMD data quality report template	
