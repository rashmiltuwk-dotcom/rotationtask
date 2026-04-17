S_prep = [];
S_prep.D = D1; 
S_prep.task = 'definetrial';
% Tell SPM to look at your specific trigger channels
S_prep.chanlabels = {'T2', 'T3', 'T6', 'T7', 'T8', 'T9', 'T10'};
D1 = spm_eeg_prep(S_prep);
save(D1); % Save the events into the metadata
