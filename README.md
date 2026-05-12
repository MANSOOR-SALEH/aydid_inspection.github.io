# AYDID Cleanroom Annotation Dashboard 🎙️

An optimized, client-side data curation and schema-alignment workbench built specifically for managing the **Arabic Yemen Dialect Identification Dataset (AYDID)**. This tool provides a real-time validation workspace that processes single-speaker regional audio files, automatically repairs missing attributes, and normalizes linguistic meta-data tags through structured controls.

---

## 🚀 Core Architectural Features

* **Dynamic Schema Injection:** Reads input CSV headers on file load. If tracking columns are absent from your initial data preparation step, the application automatically mounts them into runtime memory structure maps.
* **Redundancy Reduction:** Promotes constant global metrics (`Speaker ID`, `Gender`, `Dialect Domain`) up to a primary Session Banner view, removing repetitive field rendering across active data rows.
* **Acoustic Target Pipelines:** Generates absolute validation routing references to local storage directories matching the structure format:  
    `WAVS/{dialect}/{speaker_id}/{wav_name}`
* **Zero-Dependency Engine:** Clean, client-side architecture containing lightweight `TailwindCSS` styling, `Inter` fonts typography layout rules, and pure vanilla JS serialization loops. No local storage security configuration overrides or web servers are required.

---

## 📊 Standardized Field Mapping & Constraints

The interface applies the following strict structural constraints and UI mutations over your dataset layout model across pages of exactly **10 records**:

| Target CSV Column | UI Representation | Data Constraints & Normalization Rules |
| :--- | :--- | :--- |
| **`Retain?`** | Select Dropdown Combo | Toggles between `reserve` and `discard`. Defaults to **`reserve`** upon initial verification import. |
| **`Dur.`** | Sanitized Text Field | Records numerical length tracking contexts. Commas are stripped out on update. |
| **`Age Group`** | Select Dropdown Combo | Restricts categorical values to:<br>• `child` ($<15$)<br>• `young-adult` ($15-31$)<br>• `middle-aged` ($31-55$)<br>• `old` ($>55$) |
| **`Scripting`** | Select Dropdown Combo | Validates content alignment depth: `full`, `simi`, or `none`. |
| **`Source Type`** | Select Dropdown Combo | Categorizes recording pipeline environment: `Youtube`, `Smart Phone`, `TV Broadcast`, `Radio Content`, or `Direct Interview`. |
| **`BG Noise`** | Select Dropdown Combo | Evaluates acoustic purity values: `clear`, `some noise`, `noisy`, or `music background`. |
| **`dialect keys`** | Structured Text Input | Stores fine-grained sub-dialect structural traits (e.g., *Sanaani*, *Adeni*, *Hadrami*, etc.). |
| **`script`** | Right-to-Left (RTL) Input | RTL text input field with dedicated sizing layout specifically tuned for Arabic Transcription text strings. |
| **`English Translation`** | Inline Text Box | High-contrast input sector for structural semantic mapping. |
| **`Delete Clip`** | Dual Radio Field State | Mutually exclusive toggle between `Keep` and `DEL`. Default position is persistently unchecked. Rows marked for deletion highlight in light crimson red. |

---

## 🛠️ Data Pipeline Lifecycle Flow
