### Ecall interface

| Index | Name                            | Description                                                          | Signature                                  |
|-------|---------------------------------|----------------------------------------------------------------------|--------------------------------------------|
| 0x0   | JudgePower                      | Used to decide if the enclave is already active on initialization    | int(void)                                  |
| 0x1   | SaveCaliToLocalFile_E           | Saves calibration data                                               |                                            |
| 0x2   | Attach_E                        | Used to initialize algorithm?                                        |                                            |
| 0x3   | Detach_E                        |                                                                      | int(int *internal_err)                     |
| 0x4   | ClearContext_E                  |                                                                      | int(int *internal_err)                     |
| 0x5   | CheckUpdateArgument_E           |                                                                      |                                            |
| 0x6   | CheckEnrollmentTemplate_E       |                                                                      |                                            |
| 0x7   | DestroyEnrollmentTemplate_E     |                                                                      |                                            |
| 0x8   | InitPreProcessor_E              |                                                                      |                                            |
| 0x9   | PreProcessor_E                  |                                                                      |                                            |
| 0xA   | PreProcessorRelease_E           |                                                                      |                                            |
| 0xB   | JudgeQuality_E                  |                                                                      |                                            |
| 0xC   | CreateEnrollment_E              |                                                                      |                                            |
| 0xD   | MergeFeatureSetWithEnrollment_E |                                                                      |                                            |
| 0x17  | ?                               | Used directly after creating enclave. Driver checks output int != 0. | int(int *internal_err)                     |
| 0x19  | SendEnMessage                   |                                                                      | int(int *internal_err, char *str, int len) |
