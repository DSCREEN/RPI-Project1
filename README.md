# RPI-Project1
NVD_OTX dataset will be used to determine to what extent the type of attack vector, specifically whether local or network based influence the EPSS score.

Cleaning Dataset
I use only entries that include CVSS v3 and starts from 2016, because CVSS v2 was only used through 2015 and standards have changed since that time.
Removed years 1999 - 2015 from the dataset
for i in df_d.columns:

    if 'twitter' in i or 'tweet' in i or 'date' in i or 'attack_t' in i or 'nvd_cwe_' in i or 'nvd-cwe-' in I or 'v2' in i or ‘/’ in i or ‘\’ in I or ‘:’ in i:

        df_d.drop(i, axis=1, inplace=True)

    else:

        print(i)
