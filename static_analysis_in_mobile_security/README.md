# Static Analysis in Mobile Security

This directory contains the static analysis solutions for Android application security challenges.

## Task 0: Android App Security
- **Objective:** Decompile the target Android application (`mobile-task0.apk`) and extract the hidden flag using static analysis techniques.
- **Tools Used:** JADX-GUI (for decompiling the APK into readable Java/Kotlin code).
- **Analysis Details:**
  - Located the `MainActivityKt` within the `com.holberton.task1` package.
  - Inspected the Jetpack Compose `FlagChallenge` function.
  - Reconstructed the final flag by decoding the hardcoded Hex strings and analyzing the redundant XOR obfuscation layers (`xorDeobfuscate` combined with `xorObfuscate` using key `42`).

The decrypted flag has been saved into `0-flag.txt`.
EOF

