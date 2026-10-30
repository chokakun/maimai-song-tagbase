# 標籤字典

[回到首頁](../README.md)

以下為資料快照的字典；父子標籤不應視為獨立能力證據。

## 滑條發動與速度

識別碼：`family.slide_timing`

定義：此面向的父分類；查詢展開子標籤，不重複計算能力。

反例：父子同時出現不代表兩份獨立證據。

父分類：無

## 滑條路徑

識別碼：`family.slide_shape`

定義：此面向的父分類；查詢展開子標籤，不重複計算能力。

反例：父子同時出現不代表兩份獨立證據。

父分類：無

## 點滑複合

識別碼：`family.slide_coordination`

定義：此面向的父分類；查詢展開子標籤，不重複計算能力。

反例：父子同時出現不代表兩份獨立證據。

父分類：無

## 點打配置

識別碼：`family.tap_sequences`

定義：此面向的父分類；查詢展開子標籤，不重複計算能力。

反例：父子同時出現不代表兩份獨立證據。

父分類：無

## HOLD 複合

識別碼：`family.hold`

定義：此面向的父分類；查詢展開子標籤，不重複計算能力。

反例：父子同時出現不代表兩份獨立證據。

父分類：無

## TOUCH 配置

識別碼：`family.touch`

定義：此面向的父分類；查詢展開子標籤，不重複計算能力。

反例：父子同時出現不代表兩份獨立證據。

父分類：無

## 節奏結構

識別碼：`family.rhythm`

定義：此面向的父分類；查詢展開子標籤，不重複計算能力。

反例：父子同時出現不代表兩份獨立證據。

父分類：無

## 空間與操作範圍

識別碼：`family.spatial`

定義：此面向的父分類；查詢展開子標籤，不重複計算能力。

反例：父子同時出現不代表兩份獨立證據。

父分類：無

## 讀圖負荷

識別碼：`family.reading`

定義：此面向的父分類；查詢展開子標籤，不重複計算能力。

反例：父子同時出現不代表兩份獨立證據。

父分類：無

## 難點分布與持續性

識別碼：`family.distribution`

定義：此面向的父分類；查詢展開子標籤，不重複計算能力。

反例：父子同時出現不代表兩份獨立證據。

父分類：無

## 海底譚型點滑

識別碼：`pattern.umiyuri`

定義：限定型：兩位置每拍各一星頭／單點並交替星頭角色，半拍中間恰一個單點，至少4組；前一滑條於下一組發動。不是所有海底譚變體。
原始完整規則：Scoped recurring-pair form: at least four one-beat star/tap pairs at two positions, alternating which position is the star, with exactly one intervening tap at each half beat. The previous slide launches at the next pair within two microseconds of timing rounding. Each star links one path; extra intervening inputs break the form. Rotation, reflection and path shapes are unrestricted; omitted taps and changing pair positions are outside this version. This is an experimental form of the named family, not a complete or independently reviewed community classifier.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Any generic slide/tap overlap is insufficient. / Song-title matching must never assign this tag. / Name attestation is not detector validation.

父分類：點滑複合

## 雙位置交互

識別碼：`pattern.two_position_alternation`

定義：至少6個單輸入A/B交替，兩位置不同，等拍距，間隔不超過1拍且1秒；同時押中斷。
原始完整規則：At least six monophonic A/B onsets, distinct buttons, exactly equal rational beat gaps no greater than one beat and no greater than one second. Split at simultaneous onsets.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Two notes alone are not a trill. / Simultaneous A+B chords are not an alternating stream. / Do not infer actual left/right hand assignment.

父分類：點打配置

## 同位置連打

識別碼：`pattern.same_position_repetition`

定義：同一按鍵至少3個連續單輸入，各間隔大於0且不超過1秒；長押只算一次起音。
原始完整規則：At least three consecutive monophonic button onsets at one position, each positive gap at most one second. A sustained hold is a single onset.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 One hold is not repeated tapping. / Duplicate parser events must be removed before detection.

父分類：點打配置

## 短長節奏對

識別碼：`pattern.gallop_pairs`

定義：至少3組重複短長拍距，長短比2或3，短距不超過半拍，任何間隔不超過1拍且1秒。
原始完整規則：At least three single-input short-long pairs with exact recurring beat gaps, a long/short ratio of 2 or 3, a short gap at most half a beat, and every gap at most one beat and one second. Simultaneous inputs split a run.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 A uniform trill is not a gallop. / Three notes are not automatically musical triplets. / Do not equate every swung rhythm with this motif.

父分類：節奏結構

## 三音短爆發

識別碼：`pattern.three_note_burst`

定義：恰3個單輸入，內間距不超過四分之一拍且250ms；兩側都須有足夠分隔，截斷於曲邊界不算。
原始完整規則：Exactly three consecutive single inputs, each inner gap at most a quarter beat and 250 ms. Both neighboring gaps must be at least half a beat and twice the larger inner gap; clipped boundary triples do not qualify.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 A group of three is not necessarily triplet subdivision. / Chord cardinality is not sequential burst length.

父分類：節奏結構

## 三連音格連續配置

識別碼：`pattern.triplet_grid`

定義：至少6個等距單輸入，拍距1/3、1/6或1/12，間隔不超過1秒；單一三連短爆發不足。
原始完整規則：At least six consecutive single inputs on the authored beat grid, equally spaced by 1/3, 1/6 or 1/12 beat, with every gap at most one second. A three-note burst alone is insufficient; no audio downbeat is inferred.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Unknown beat anchor yields unknown. / Three arbitrary notes do not establish triplet rhythm.

父分類：節奏結構

## 連續半拍相位起音

識別碼：`pattern.offbeat_onsets`

定義：至少4個單輸入都位於轉寫拍格的半拍相位，間隔恰1拍且不超過2秒；不據此宣稱音樂切分。
原始完整規則：At least four consecutive single inputs at the half-beat phase of the authored grid, exactly one beat apart and at most two seconds apart. This is a notation-grid observation, not a claim of musical syncopation.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 BPM alone does not establish the musical downbeat. / Do not call a chart syncopated solely from a shifted global offset.

父分類：節奏結構

## 同時押

識別碼：`pattern.simultaneous_group`

定義：至少2個不同輸入共用明示同時群；僅時間戳相同不足。
原始完整規則：Two or more distinct input onsets with one explicit authored simultaneous-group ID. Equal timestamps alone are insufficient.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Near-simultaneous decorative notes are not necessarily a chord. / A shared slide head is not several taps.

父分類：點打配置

## 連續同時押

識別碼：`pattern.chord_stream`

定義：至少3個連續明示同時群，每組至少2輸入，正的等拍距不超過1拍且1秒。
原始完整規則：At least three consecutive authored simultaneous groups, each containing at least two inputs, with equal positive beat gaps no greater than one beat or one second. Group sizes and button shapes may differ.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Do not claim a fixed two-hand solution. / Different group shapes are retained, not flattened.

父分類：點打配置

## 相鄰階梯點打

識別碼：`pattern.tap_staircase`

定義：同方向相鄰移動4至7個單點／星頭，間隔不超過1拍且1秒；8個以上另列外圈旋轉。
原始完整規則：A maximal run of four to seven single tap/star inputs stepping to adjacent buttons in one circular direction. Gaps are at most one beat and one second. Runs of eight or more inputs are perimeter runs instead.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 One long slide is not a tap staircase. / Do not prescribe a hand crossover.

父分類：點打配置

## 外圈連續旋轉

識別碼：`pattern.perimeter_run`

定義：至少8個相鄰同方向單點／星頭，走遍外圈，間隔不超過1拍且1秒。
原始完整規則：At least eight consecutive single tap/star inputs visiting the full button ring in one direction, with adjacent steps and gaps at most one beat and one second. Circular wraparound is retained.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Visual rotation alone is insufficient. / A fan slide is not a perimeter tap run.

父分類：點打配置

## 點打方向反轉

識別碼：`pattern.direction_reversal`

定義：相鄰單點同方向至少2步後折返至少2步；雙位置交互排除。
原始完整規則：A consecutive single tap/star neighbor run changes direction after at least two steps and continues at least two steps in the opposite direction. Gaps are at most one beat and one second; a two-position trill is excluded.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 One repeated button is not a direction change. / The shortest geometric path need not be the player hand path.

父分類：空間與操作範圍

## 同起點分岔滑條

識別碼：`pattern.same_head_slide_fan`

定義：一顆既有星頭連接至少2條不同路徑；星頭輸入只算一次。
原始完整規則：At least two path IDs sharing one existing star-tap head; count that input once.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Different heads at the same timestamp are not a shared head. / Multiple branches do not prove more hands are required.

父分類：滑條路徑

## 錯開滑條起點

識別碼：`pattern.staggered_slide_starts`

定義：至少2條滑動區間互相連通且移動開始時刻不同；只等待、只碰端點不算。
原始完整規則：A connected interval contains at least two moving slide paths with different movement start times. Waiting stars alone and paths that only touch at an endpoint do not qualify. Shared-head branches may qualify.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Simultaneous visual appearance is not movement overlap. / A slide waiting to move must not be counted as already moving.

父分類：滑條發動與速度

## 多條滑動區間重疊

識別碼：`pattern.moving_slide_overlap`

定義：至少2條實際移動的半開區間有正長度交集；端點相接不算。
原始完整規則：Maximal connected intervals with at least two active half-open slide movements; touching endpoints do not overlap.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Waiting intervals are separate. / Concurrency does not prove crossing hands or occlusion.

父分類：讀圖負荷

## 滑動期間夾點

識別碼：`pattern.slide_tap_interleave`

定義：獨立點打／星頭落在滑條半開移動區間內；泛型點滑關係，不能直接推為海底譚。
原始完整規則：At least one independent tap/star input inside a half-open slide movement. Generic interaction only; this is not an Umiyuri recognizer.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 This is not sufficient for the Umiyuri tag. / Temporal overlap alone does not establish two independent hand actions.

父分類：點滑複合

## 滑條等待期間夾點

識別碼：`pattern.delayed_slide_interleave`

定義：獨立點打落在滑條半開等待區間，排除自己星頭及等待結束端點。
原始完整規則：At least one independent tap/star input inside a half-open slide wait, excluding its own shared head and the wait-end boundary.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Taps during movement belong to a different detector. / Default delay alone is not automatically unusual timing.

父分類：點滑複合

## 等待長度變化

識別碼：`pattern.variable_slide_wait`

定義：至少3個連續不同滑條星頭，等待拍數差至少四分之一拍，星頭相隔最多4拍且4秒；同拍數隨BPM改變秒數不算。
原始完整規則：At least three consecutive distinct slide heads have positive waits whose lengths differ by at least a quarter beat, allowing two microseconds of clock rounding. Heads are at most four beats and four seconds apart. A tempo map is required; equal beat waits at changing BPM are not variable waits. Heads whose branches have different waits split the sequence.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Tempo change can alter seconds without changing beat-relative structure. / Unsupported waiting syntax produces unknown.

父分類：滑條發動與速度

## 連接滑條

識別碼：`pattern.connected_slide_chain`

定義：同一條路徑含至少2個明示有序連接段；連接段不增加實際輸入起音。
原始完整規則：One normalized path with at least two explicitly ordered connected segment IDs. Segments never create additional physical input onsets.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Adjacent unrelated slides are not automatically one connected chain. / Segment count is not note count.

父分類：滑條路徑

## HOLD 中夾點

識別碼：`pattern.hold_tap_interleave`

定義：獨立點打／星頭落在HOLD半開持續區間內。
原始完整規則：At least one independent tap/star input during a half-open held interval.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Do not assign a holding hand from aggregate geometry alone.

父分類：HOLD 複合

## HOLD 與滑條重疊

識別碼：`pattern.hold_slide_overlap`

定義：HOLD與滑條實際移動有正長度交集；不含只等待或端點相接，不指定雙手分工。
原始完整規則：A positive-length, half-open held interval overlaps a slide's movement. Waiting slides and touching endpoints do not qualify. No mandatory hand assignment is inferred.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Overlap is a structural observation, not proof of an impossible input combination.

父分類：HOLD 複合

## 外圈點打與 TOUCH 交錯

識別碼：`pattern.touch_tap_interleave`

定義：至少4個單輸入在TOUCH類與外圈點打／星頭間交替，間隔不超過半拍且1秒；同時群排除。
原始完整規則：At least four consecutive single inputs alternate between a touch/touch-hold onset and a tap/star button input, with positive gaps at most half a beat and one second. Simultaneous touch/button chords do not count as alternation.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Touch/button switching is not measured hand travel. / Missing touch-zone geometry limits movement interpretations.

父分類：TOUCH 配置

## 高起音密度

識別碼：`trait.high_onset_density`

定義：完整1秒窗至少12個實際輸入、至少4個不同時點；窗每250ms前進；描述輸入率，不等於難度。
原始完整規則：A complete one-second window contains at least 12 physical input onsets at four or more distinct times. Windows advance by 250 ms; overlapping hits merge. This absolute threshold describes input rate, not player difficulty.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Break score value is not extra physical note count. / This does not measure total difficulty.

父分類：點打配置

## 短時間密度爆發

識別碼：`trait.bursty_density`

定義：完整觀察範圍至少4秒、8個起音，250ms峰值至少全曲均值2倍，且多4輸入/秒。
原始完整規則：Fully covered chart spans at least four seconds and has at least eight onsets; 250 ms peak density is at least twice the chart mean and exceeds it by four onsets/s. Measured over the observed chart span; unknown leading/trailing audio silence is excluded.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Very low baseline alone must not produce a dramatic burst label. / A density burst is not a diagnosis of stamina demand.

父分類：難點分布與持續性

## 持續密集起音

識別碼：`trait.sustained_density`

定義：至少連續4個完整1秒格，每格至少8輸入且4個不同時點；缺資料或較低密度會中斷。
原始完整規則：At least four consecutive complete one-second bins each contain eight or more inputs at four or more distinct times. Bins start at the observed chart start. Missing time or a lower-density bin splits a stretch.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Unknown chart span must be reported. / Long holds alone do not establish high onset density.

父分類：難點分布與持續性

## 尾段起音較密

識別碼：`trait.backloaded_density`

定義：尾三分之一的起音率至少前段1.5倍，且多2輸入/秒；不直接稱尾殺。
原始完整規則：Fully covered chart has at least eight onsets; final-third onset rate is at least 1.5 times first-third and at least two onsets/second greater. Not a hard-ending claim. Measured over the observed chart span; unknown leading/trailing audio silence is excluded.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Call this backloaded density, not guaranteed ending difficulty. / An uncertain audio tail must not shift classification silently.

父分類：難點分布與持續性

## 前段起音較密

識別碼：`trait.frontloaded_density`

定義：前三分之一的起音率至少尾段1.5倍，且多2輸入/秒。
原始完整規則：Fully covered chart has at least eight onsets; first-third onset rate is at least 1.5 times final-third and at least two onsets/second greater. Measured over the observed chart span; unknown leading/trailing audio silence is excluded.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Song audio duration and note span are not interchangeable.

父分類：難點分布與持續性

## 單一密度尖峰

識別碼：`trait.isolated_density_spike`

定義：全曲內部恰1組高峰，至少8輸入/秒且為1秒格中位數2倍，前後皆較低；不推定得分難點。
原始完整規則：Exactly one interior group of one-second bins reaches at least eight inputs/s and twice the median bin count of a fully observed chart span. Lower bins bracket it; a peak is not a difficulty or scoring claim.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Do not smooth away a short spike. / This tag says nothing about pattern teachability without separate evidence.

父分類：難點分布與持續性

## 多段密度高峰

識別碼：`trait.multi_peak_density`

定義：至少2組符合上述內部峰值規則的高峰，兩峰之間至少1個較低格。
原始完整規則：Two or more interior groups meet the same peak rule: at least eight inputs/s and twice the median one-second bin count, with a lower bin on both sides and at least one lower bin between groups, over a fully observed chart span.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Tiny numerical ripples are not separate meaningful peaks.

父分類：難點分布與持續性

## 起音密度穩定

識別碼：`trait.steady_density`

定義：至少4秒、8個起音；24等時段密度變異係數≤0.2且均值&gt;0。
原始完整規則：Fully covered chart spans at least four seconds and has at least eight onsets; 24 segment density coefficient of variation is at most 0.2, with positive mean. Measured over the observed chart span; unknown leading/trailing audio silence is excluded.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 An empty chart is not a steady practice chart. / Steady density does not imply easy execution.

父分類：難點分布與持續性

## 低起音密度空檔

識別碼：`trait.low_onset_gaps`

定義：至少連續2個完整1秒格各最多1個新輸入；可能仍在滑／HOLD，不當作休息。
原始完整規則：At least two consecutive complete one-second bins contain at most one new input each, in a chart with at least four observed inputs. Ongoing holds and slides may remain, so this does not claim a rest or recovery opportunity.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Low onset count during ongoing slides is not necessarily a rest.

父分類：難點分布與持續性

## BREAK 集中

識別碼：`trait.break_concentration`

定義：4秒窗至少4個BREAK輸入、占全曲BREAK至少40%，窗內BREAK比例至少25%且為全曲1.5倍；不含Rating加權。
原始完整規則：A four-second window contains at least four break inputs, at least 40% of the chart's break inputs, and a break fraction of at least 25% and 1.5 times the chart-wide fraction. Windows advance by one second; overlapping hits merge. Counts concern break input flags, not rating-weighted scoring objects.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Break value must not inflate physical density. / Scoring risk requires a separate version-aware rating/scoring interpretation.

父分類：難點分布與持續性

## 起音間隔多變

識別碼：`trait.rhythm_variability`

定義：至少12個連續單輸入，間隔最多1拍且1秒，至少2種拍距，拍距變異係數≥0.35，至少35%轉換改變間距。
原始完整規則：At least 12 consecutive single inputs have positive gaps no greater than one beat or one second, two or more distinct beat gaps, coefficient of variation at least 0.35, and changed spacing at at least 35% of transitions. Beat units prevent tempo changes alone from creating variability.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Entropy alone is not musical complexity. / Tempo changes are not automatically harder rhythm.

父分類：節奏結構

## 滑動時間占比高

識別碼：`trait.slide_occupancy`

定義：滑條實際移動區間的聯集覆蓋已觀察全曲範圍至少一半；重疊時間不重複加總。
原始完整規則：At least one moving path occupies at least half of the fully covered chart span; overlapping paths do not double the occupied duration. Measured over the observed chart span; unknown leading/trailing audio silence is excluded.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Many visible waiting slides are not moving occupancy. / High occupancy does not imply a named motif.

父分類：滑條發動與速度

## 配置重複出現

識別碼：`trait.repeated_motif`

定義：兩個不重疊8組起音片段各長2至8拍，拍距、角色、位置、旗標、HOLD與滑條時長、路徑字串相同；不推定鏡像或手法等價。
原始完整規則：Two disjoint eight-onset-group phrases, spanning two to eight beats, have the same beat gaps, input roles, positions, flags, hold lengths and slide wait/movement lengths and source path strings. Phrases require at least two input positions or roles; single repeated-button streams are excluded. Slide paths must be present. Exact layout only; no reflection or playable-strategy equivalence is inferred.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Rotation and reflection are not always equally playable. / Shared broad tags are not sufficient to assert repetition.

父分類：讀圖負荷

## 配置集中於獨立段落

識別碼：`trait.isolated_pattern_sections`

定義：指定配置至少250ms、3輸入；沒有不相關HOLD／滑動重疊，區間額外輸入≤20%，周圍半秒最多2個額外輸入；不代表訓練成效。
原始完整規則：A supported input pattern spanning at least 250 ms and three inputs has no unrelated overlapping hold/slide movement, at most 20% extra inputs inside it, and at most two extra inputs in its half-second surroundings. This is target-specific isolation, not evidence of training effectiveness.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 This is target-specific, not a universal chart property. / Isolation supports a practice hypothesis; it does not prove learning effectiveness.

父分類：難點分布與持續性

## 固定軸交互

識別碼：`pattern.anchored_trill`

定義：至少8個規律交互輸入，一側固定軸，另一側至少3種移動位置。
原始完整規則：At least eight equally spaced single button inputs alternate a fixed anchor with a moving position. At least three distinct non-anchor positions occur. Gaps are at most half a beat and one second; chords split the sequence.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：點打配置

## 散打連續配置

識別碼：`pattern.scattered_taps`

定義：至少8個等距單點、4個位置且至少3種非相鄰跳躍；固定軸交互另列。
原始完整規則：At least eight equally spaced consecutive single tap/star inputs visit at least four buttons, with gaps at most half a beat and one second. At least three transitions jump to a distinct non-neighboring button. Fixed-anchor alternations are excluded. This scoped scattered-stream rule is not a catch-all difficulty label.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：點打配置

## 連續 TOUCH

識別碼：`pattern.touch_stream`

定義：至少6個連續單顆TOUCH、至少3個感應位置；TOUCH HOLD／同時群中斷。
原始完整規則：At least six consecutive single touch onsets visit at least three zones, with gaps at most half a beat and one second. Button inputs, touch holds and simultaneous touches split the stream.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：TOUCH 配置

## TOUCH 階梯

識別碼：`pattern.touch_sweep`

定義：同一感應圈4至7個連續相鄰單顆TOUCH；跨圈或中心會中斷。
原始完整規則：A maximal run of four to seven single touch inputs steps between neighboring numbered zones on the same A, B, D or E ring in one direction. Gaps are at most half a beat and one second. Central and cross-ring touches split the sequence.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：TOUCH 配置

## TOUCH 旋轉

識別碼：`pattern.touch_rotation`

定義：同一感應圈至少8個連續相鄰單顆TOUCH；跨圈或中心會中斷。
原始完整規則：At least eight consecutive single touch inputs traverse one numbered A, B, D or E ring in one direction with adjacent steps. Gaps are at most half a beat and one second. Central and cross-ring touches split the sequence.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：TOUCH 配置

## 同位置反覆滑條起點

識別碼：`pattern.repeated_slide_heads`

定義：同位置至少3個等距、各連一條路徑的不同星頭。
原始完整規則：At least three consecutive distinct slide heads at one button, spaced equally by at most one beat and one second. Each head owns exactly one path. Additional non-slide inputs split the sequence. One shared branching head is not repeated heads.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：滑條發動與速度

## 雙位置交替滑條起點

識別碼：`pattern.alternating_slide_heads`

定義：至少4個等距、各連一條路徑的星頭，在兩個固定位置交替。
原始完整規則：At least four consecutive single-path slide heads alternate between two distinct buttons, with equal gaps at most one beat and one second. Additional non-slide inputs and branching heads split the sequence.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：滑條發動與速度

## 等長路徑同時異速

識別碼：`pattern.different_slide_speeds`

定義：同時發動的兩條等長簡單路徑，移動時長比例至少1.25；不同路徑長度不能單憑時值比較。
原始完整規則：Two authored simultaneous single-path slide heads launch together within two microseconds. Their simple paths have equal shape length under rotation/reflection, but movement durations differ by a ratio of at least 1.25. Unequal-length and connected paths are outside this form; differing durations alone do not establish different speed.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：滑條發動與速度

## 延長等待發動

識別碼：`pattern.extended_slide_wait`

定義：滑條等待嚴格超過當時1拍，容許2微秒四捨五入。
原始完整規則：A slide waits more than one authored beat between its wait start and movement start, allowing two microseconds of clock rounding. Requires a covering tempo map. A normal one-beat wait at a slow BPM is excluded.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：滑條發動與速度

## 原路折返滑條

識別碼：`pattern.return_slides`

定義：連續兩條簡單直線或圓弧沿同一路徑反向，生命區間重疊。
原始完整規則：Two consecutive simple straight or arc slides retrace the same path in opposite directions. The second head arrives after the first, no more than two beats and two seconds later, while their wait/movement lifetimes overlap. Merely crossing paths do not qualify.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：滑條路徑

## CYCLES 型配置

識別碼：`pattern.cycles`

定義：至少3組固定對向星頭的EACH，圓弧對與p/q迴環對交替；限定結構型，不按曲名判定。
原始完整規則：At least three consecutive equally spaced two-head EACH slide groups at fixed opposite buttons alternate between two arcs and two p/q loops. Each head owns one simple path; launches are paired. Group gaps are at most one beat and one second. This recognizes an arc-pair/loop-pair form, not all CYCLES variants.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：點滑複合

## Slip Flip 型配置

識別碼：`pattern.slip_flip`

定義：至少3組固定對向星頭的圓弧／迴環混合EACH，角色持續固定；與CYCLES型分開。
原始完整規則：At least three consecutive equally spaced EACH slide pairs at fixed opposite buttons each combine one simple arc and one p/q loop. The arc and loop retain their respective head positions; paired launches coincide. Group gaps are at most one beat and one second. This mixed-pair form is distinct from CYCLES.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：點滑複合

## Death Scythe 型配置

識別碼：`pattern.death_scythe`

定義：至少8個相鄰外圈連續輸入，至少2個反方向圓弧星頭各與其他輸入重疊。
原始完整規則：A single-input button run of at least eight adjacent steps in one direction contains at least two simple arc slide heads whose arcs travel in the opposite direction. Each arc overlaps an independent input in that run. Input gaps are at most half a beat and one second. Straight slides and mere tap/slide overlap do not qualify.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：點滑複合

## Sugarbitter 型配置

識別碼：`pattern.sugarbitter`

定義：至少3個同按鍵星頭，每個都同時發動兩條不同直線分支。
原始完整規則：At least three equally spaced consecutive heads at one button each share exactly two distinct simple straight slide branches with simultaneous launches. Gaps are at most one beat and one second. One fan or repeated unbranched slides do not establish this form.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：點滑複合

## Future 白譜型配置

識別碼：`pattern.future`

定義：至少3組每拍星頭／點打EACH，後組點打回到前星頭位置，前滑條在下一組發動。
原始完整規則：At least three consecutive one-beat EACH groups contain one single-path slide head and one tap. Slide heads change position; each later tap revisits the previous head, and the previous slide launches at the next group within two microseconds. No intervening onsets are allowed. This positional form does not infer a required hand switch.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：點滑複合

## 激唱型連結掃鍵

識別碼：`pattern.gekishou`

定義：至少兩段短而互斥、反向的相鄰掃鍵，共用明示EACH端點。
原始完整規則：At least two consecutive short neighbor sweeps share EACH endpoints. Each sweep has three or four inputs with equal gaps at most a quarter beat and one second. Successive sweeps travel in opposite directions, use different endpoint notes at their shared chord, and occupy disjoint button sets. Hands are not inferred.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：點打配置

## 星空型相對位置序列

識別碼：`pattern.hoshizora`

定義：六輸入相對位置型1,3,5,1,7,5，允許旋轉／鏡像，包含HOLD起音。
原始完整規則：Six equally spaced single button onsets follow the relative position sequence 1,3,5,1,7,5, allowing rotation and reflection. Tap, star and hold onsets qualify; gaps are at most half a beat and one second. This source-observed six-input form is not a general classifier of crossing or required hands.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：點打配置

## Outlaw 型移位掃鍵

識別碼：`pattern.outlaw`

定義：短相鄰掃鍵以EACH端點連接，方向長度相同，各段起點移一鍵。
原始完整規則：At least two consecutive three- or four-input neighbor sweeps share EACH endpoints, using different notes at each shared chord. Their directions and lengths agree, while each successive starting button moves one neighbor step in that direction. Equal gaps are at most a quarter beat and one second.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：點打配置

## 連續附點八分間隔

識別碼：`pattern.amazing_mightyyy`

定義：至少5組起音，相隔四分之三拍；附點八分連續型。
原始完整規則：At least five consecutive authored onset groups are separated by exactly three quarters of a beat and at most one second. Chords may occur within a group. This dotted-eighth timing form does not require the source song or a specific hand assignment.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：節奏結構

## 旋轉直徑滑條

識別碼：`pattern.magic_circle`

定義：至少4條跨直徑直線，各起點依同方向移動相鄰一鍵。
原始完整規則：At least four consecutive equally spaced single-head straight slides each connect opposite buttons. Starting positions progress by one adjacent button in a consistent circular direction. Gaps are at most one beat and one second. Parallel or arbitrary diagonal slides do not establish the progression.

反例：不符合上述最小長度、節奏、位置或區間條件的相似配置不算；不推定玩家手法或能力。 Recognition covers the stated structural form; community variants and compulsory hands are not inferred.

父分類：滑條路徑

## 短等待發動

識別碼：`local.short_wait`

定義：非連接段滑條等待嚴格小於當時1拍。

反例：正常一拍等待不屬於短等待。

父分類：滑條發動與速度

## 慢速滑動

識別碼：`local.slow_slide`

定義：簡單直線或圓弧的理想圖形路徑長度／移動秒數 ≤ 2.5 R/s；R為圓盤半徑。

反例：低BPM、長時值本身不足；其他路徑未量測不判為無。

父分類：滑條發動與速度

## 快速滑動

識別碼：`local.fast_slide`

定義：同一理想圖形速度 ≥ 6 R/s；不代表手實際移動速度。

反例：短路徑短時值不一定快。

父分類：滑條發動與速度

## 等長路徑同時同速

識別碼：`local.same_speed`

定義：兩條等長簡單路徑的發動與結束時間各相差不超過2微秒。

反例：只有同時出現、路徑長度不同者不算。

父分類：滑條發動與速度

## 連續滑條速度變化

識別碼：`local.speed_changes`

定義：連續至少3條可量測路徑，兩次相鄰速度比皆 ≥ 1.5，起點間隔 ≤ 2秒。

反例：只比較BPM或滑條時值不算。

父分類：滑條發動與速度

## 直線滑條

識別碼：`local.straight`

定義：單段路徑記法為 -。

反例：連接路徑含直線段不等於整條直線。

父分類：滑條路徑

## 圓弧滑條

識別碼：`local.arc`

定義：單段記法為 &lt;、&gt; 或 ^。

反例：p/q迴環另列，不直接當圓周圓弧。

父分類：滑條路徑

## 折線滑條

識別碼：`local.polyline`

定義：單段 v、V、s 或 z 記法。

反例：曲線路徑不算折線。

父分類：滑條路徑

## 直線跨中心

識別碼：`local.diameter`

定義：直線起終點在外圈正對面，相距4鍵。

反例：跨畫面但未經中心不算。

父分類：滑條路徑

## 長距離圓弧

識別碼：`local.long_arc`

定義：可辨識圓周圓弧沿途經過至少半圈。

反例：p/q迴環沒有確定幾何不據此量測。

父分類：滑條路徑

## 扇形滑條

識別碼：`local.wifi`

定義：單段記法為 w。

反例：同起點兩條普通滑條不是wifi。

父分類：滑條路徑

## 迴環滑條

識別碼：`local.loop`

定義：單段記法為 p/q/pp/qq。

反例：普通圓弧不當成迴環。

父分類：滑條路徑

## 發動瞬間夾點

識別碼：`local.tap_at_launch`

定義：獨立點打距滑條移動開始 ≤ 2毫秒，排除自己的星頭。

反例：等待區間中的點打另列。

父分類：點滑複合

## 收尾瞬間夾點

識別碼：`local.tap_at_end`

定義：獨立點打距滑條結束 ≤ 2毫秒。

反例：滑條中途點打不算收尾。

父分類：點滑複合

## 滑動期間連續點打

識別碼：`local.tap_run_slide`

定義：一條滑動區間內至少3個獨立點打起音，間隔皆 ≤ 0.5秒。

反例：三顆同時押只有一組時點不算連續。

父分類：點滑複合

## 滑動期間同時押

識別碼：`local.chord_slide`

定義：滑動區間內存在至少2個不同輸入的明示同時群，排除自身星頭。

反例：同時星頭本身不算滑動期間額外同時押。

父分類：點滑複合

## 多條滑動期間夾點

識別碼：`local.multi_slide_tap`

定義：一個獨立點打同時落在至少2條半開滑動區間內。

反例：只是在同一首出現兩滑與點打不算。

父分類：點滑複合

## 單點與同時押交替

識別碼：`local.single_chord_switch`

定義：連續4組起音的組大小在1與≥2之間交替，各間隔 ≤ 1秒。

反例：兩組交替不足以建立持續配置。

父分類：點打配置

## 長 HOLD

識別碼：`local.long_hold`

定義：持續長度 ≥ 2拍的外圈HOLD。

反例：TOUCH HOLD另列，低BPM的普通短HOLD不單憑秒數判斷。

父分類：HOLD 複合

## 短 HOLD 連續配置

識別碼：`local.short_hold_run`

定義：至少3個外圈HOLD起點間隔 ≤ 1秒，每個時值 ≤ 半拍。

反例：僅有三個不相鄰HOLD不算。

父分類：HOLD 複合

## 錯開放手

識別碼：`local.staggered_release`

定義：起點相同的兩個HOLD，結束時間不同且相差 &gt; 2毫秒。

反例：不同時間按下的兩HOLD不直接當成同押錯開放手。

父分類：HOLD 複合

## HOLD 中 TOUCH

識別碼：`local.hold_touch`

定義：外圈HOLD半開持續區間中出現TOUCH或TOUCH HOLD起音。

反例：HOLD放手後的TOUCH不算。

父分類：HOLD 複合

## 單點 TOUCH

識別碼：`local.touch_single`

定義：一組起音僅有一顆TOUCH，且沒有同組其他輸入。

反例：TOUCH群不是單點。

父分類：TOUCH 配置

## TOUCH 群

識別碼：`local.touch_group`

定義：同一明示同時群至少2顆TOUCH。

反例：相近但非同時的TOUCH不算。

父分類：TOUCH 配置

## TOUCH 與滑條重疊

識別碼：`local.touch_slide`

定義：TOUCH起音落在至少一條滑動半開區間中。

反例：只有同曲出現兩者不算重疊。

父分類：TOUCH 配置

## TOUCH HOLD

識別碼：`local.touch_hold`

定義：包含TOUCH HOLD事件；另外保存持續區間。

反例：外圈HOLD不是TOUCH HOLD。

父分類：TOUCH 配置

## 八分等距連續段

識別碼：`local.eighth`

定義：至少6組起音，連續間距為半拍；容許2微秒四捨五入差。

反例：BPM速度不是八分節奏的判斷。

父分類：節奏結構

## 十六分等距連續段

識別碼：`local.sixteenth`

定義：至少6組起音，連續間距為四分之一拍。

反例：僅有一組十六分間隔不算連續段。

父分類：節奏結構

## 休止後起手

識別碼：`local.rest_restart`

定義：兩組起音之間至少2拍，後者為重新起手點。

反例：它是起音空檔，期間仍可能有HOLD／滑條。

父分類：節奏結構

## 譜內變速

識別碼：`local.bpm_change`

定義：兩個相鄰BPM宣告值確實不同。

反例：重複宣告相同BPM不算變速。

父分類：節奏結構

## 相鄰區域移動

識別碼：`local.near_jump`

定義：至少4組單點輸入相鄰移動，鍵距為1且間隔 ≤ 1秒。

反例：同時押不指定兩手移動路徑。

父分類：空間與操作範圍

## 大跨度點打

識別碼：`local.far_jump`

定義：連續單點起音鍵距≥3，間隔 ≤ 半秒，至少3個起音。

反例：兩個不相鄰但間隔很久的點打不算。

父分類：空間與操作範圍

## 正對面交互

識別碼：`local.diameter_alternation`

定義：至少6個等拍距單輸入，兩個按鍵正對面相距4鍵；間隔不超過1拍且1秒。

反例：泛稱跨中心手法或不等拍距交替，不等於此雙位置交互細型。

父分類：空間與操作範圍

## 左右區域交替

識別碼：`local.lr_alternation`

定義：至少6個單點起音左右半圓交替，間隔 ≤ 1秒。

反例：同時押、換手方式不由此推定。

父分類：空間與操作範圍

## 上下區域交替

識別碼：`local.ud_alternation`

定義：至少6個單點起音上下半圓交替，間隔 ≤ 1秒。

反例：僅左右交替不算。

父分類：空間與操作範圍

## 跨區同時押

識別碼：`local.wide_chord`

定義：同時群中有兩個外圈輸入最短鍵距 ≥ 3。

反例：不宣稱必須交叉手。

父分類：空間與操作範圍

## 路徑幾何交疊

識別碼：`local.path_overlap`

定義：須有可靠路徑幾何與時間覆蓋的視覺／幾何核對。

反例：滑動時間重疊不代表路徑交疊。

父分類：讀圖負荷

## 多滑條同屏

識別碼：`local.screen_slides`

定義：須核對出現時機與遊戲顯示設定。

反例：事件移動區間不等於顯示區間。

父分類：讀圖負荷

## 起終點視覺密集

識別碼：`local.visual_clutter`

定義：須以固定顯示設定核對同屏起終點的視覺密集。

反例：只用音符總數不能判斷。

父分類：讀圖負荷

## 相似配置局部變化

識別碼：`local.similar_variation`

定義：須對照重複段落中位置或節奏的局部差異。

反例：重複配置本身不算局部變化。

父分類：讀圖負荷

## 突然切換配置

識別碼：`local.pattern_switch`

定義：須核對相鄰段落的配置要求變化。

反例：密度突然上升不等於換配置。

父分類：讀圖負荷

## 開頭主要難點

識別碼：`local.hard_start`

定義：由完整配置複核後指定，不從起音密度直接推定。

反例：前段較密不必然最難。

父分類：難點分布與持續性

## 中央主要難點

識別碼：`local.hard_middle`

定義：由完整配置複核後指定。

反例：中央音符多不等於中央最難。

父分類：難點分布與持續性

## 尾段主要難點

識別碼：`local.hard_end`

定義：由完整配置複核後指定。

反例：尾殺不能只用尾段密度代判。

父分類：難點分布與持續性

## 實際操作休息少

識別碼：`local.little_rest`

定義：須綜合點打、滑條與HOLD操作，再作配置複核。

反例：起音少的長滑條不一定是休息。

父分類：難點分布與持續性
