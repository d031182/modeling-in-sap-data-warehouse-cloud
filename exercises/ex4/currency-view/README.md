# Create Currency Views

Date: 2021-09-22

As of today, SAP Analytics Cloud must not access any table directly in SAP Data Warehouse Cloud due to security boundaries.
That applies also for the currency conversion relevant tables such as **TUCRR (Rates)**, **TCURX (Precisions)**, **TCURV (Configurations)**, **TCURF (Prefactors)**.
