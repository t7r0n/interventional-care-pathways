# Failure Matrix: Interventional Care Pathways

| Scenario | Failure mode | Metric | Gate | Evidence |
| --- | --- | --- | --- | --- |
| interventional evidence replay | interventional_drift | interventional_coverage | block release until cited evidence is regenerated | ev_0000 |
| care-pathway operator packet | care-pathway_blindspot | care-pathway_latency | accept only if decision claims cite fixture evidence | ev_0007 |
| care-pathway operator packet | care-pathway_blindspot | care-pathway_latency | accept only if decision claims cite fixture evidence | ev_0011 |
| clinics regression harness | clinics_misroute | clinics_precision | open a regression issue with trace and benchmark delta | ev_0014 |
| psychiatry boundary probe | psychiatry_gap | psychiatry_risk | route to reviewer with evidence packet | ev_0021 |
| clinics regression harness | clinics_misroute | clinics_precision | open a regression issue with trace and benchmark delta | ev_0022 |
| interventional evidence replay | interventional_drift | interventional_coverage | block release until cited evidence is regenerated | ev_0028 |
