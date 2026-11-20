# **تخصص Systems Programming & AI Inference Engineering**

سأتعامل مع هذا المسار باعتباره تخصصاً هندسياً طويل المدى، وليس خطة لتعلم Linux أو C++ أو CUDA بشكل منفصل.

الهدف النهائي الذي سنعمل للوصول إليه هو:

**أن تكون قادراً على فهم وبناء وتحسين الأنظمة التي تشغّل نماذج الذكاء الاصطناعي، ابتداءً من مستوى الذاكرة والعمليات ونظام التشغيل، وصولاً إلى Inference Engines التي تخدم نماذج LLM على GPU وتتعامل مع آلاف الطلبات.**

هذا التخصص يجمع بين ثلاثة مستويات:

## **Level 1 — Computer Systems**

كيف يعمل الكمبيوتر والبرنامج من الداخل؟

[File:Computer Systems - Von Neumann Architecture Large poster anchor chart.svg - Wikimedia Commons](https://images.openai.com/static-rsc-4/ss6mg1b040X_VTAzZiVwB8Ib1fyLSUuDCoJI5-GSDxArhqNxQ2Pq-4rTzexH4AyGaYVdegRxdbtAKkOL-wmeAtvgblkoEKU2YDbX_EB4N9naqPKesU6ufSsGQBwJwKoVxQKELT9uZnkBTKARlKsOd23_k1zjWUOgPbKOC56fe6A?purpose=inline)

[commons.wikimedia.org](https://commons.wikimedia.org/wiki/File%3AComputer_Systems_-_Von_Neumann_Architecture_Large_poster_anchor_chart.svg?utm_source=chatgpt.com)

**C · Computer Architecture · Memory · Operating Systems · Linux**

## **Level 2 — Systems Engineering**

كيف نبني برامج عالية الأداء وتعمل بالتوازي؟

[If You Understand These 20 OS Concepts, You’re Already a Better Developer Than 80% of the Industry | by ArchitectOfExperience | Medium](https://images.openai.com/static-rsc-4/IELnSi2hS4xadvIFP1pfV7xpfVe4WHXHfcgB7Ji8lCX_TGVKWUah9L1Gr4M_9gTyQQQd5MRN-BE7YHIjoDas9paq49FXilZT-0-GJGwEj5ScjvrMFHA6QGY7z3YGUob347wStgifHs5VyamdekaDcfHkGY8r2uC29SI5OA-OYME?purpose=inline)

[medium.com](https://medium.com/%40harish852958/if-you-understand-these-20-os-concepts-youre-already-a-better-developer-than-80-of-the-industry-0b76deff57d2?utm_source=chatgpt.com)

**C++ · Concurrency · Networking · Performance · GPU Programming**

## **Level 3 — AI Inference Engineering**

كيف نبني محركات تشغيل نماذج الذكاء الاصطناعي؟

[A survey on Inference Serving for Large Language Models | hello@woonyee.org \~ $](https://images.openai.com/static-rsc-4/mtI2Ym9aLJNhSDss-rjN1nDnpPN-x-172qUsrx18LLKPhGxMMrXKNTuAzSO3i0lEj80kHwGcVJMF1dcDX_0Y6RyW40amlHOHzrwN9fw-t3-zVAd0ZPsV9XTN22k_G4ehLgsgnGcZjlrOFAoEaRQmhB3XPhNuxkagDDIu2bPiYSg?purpose=inline)

[woonyee.org](https://woonyee.org/projects/ml-inference-sys-review/?utm_source=chatgpt.com)

**CUDA · LLM Inference · KV Cache · Batching · vLLM · Distributed Inference**

## **ما النتيجة التي نريد الوصول إليها؟**

في نهاية المسار، أريد أن تستطيع بناء مشروع مثل:

**Mini LLM Inference Engine**

محرك مبسط لتشغيل نموذج لغوي، يحتوي على:

- Tokenizer وModel Execution.
- إدارة الذاكرة والـ Tensors.
- GPU Kernels.
- KV Cache Management.
- Request Scheduling.
- Continuous Batching.
- Multiple Concurrent Requests.
- Performance Profiling.
- Benchmarking ومقارنة مع vLLM.

ليس المطلوب أن تنافس vLLM من البداية، وإنما أن تفهم كيف تعمل هذه الأنظمة، وتكون قادراً على بناء أجزاء منها وتحسينها.

# **أولاً: المدة وطريقة الدراسة**

أقترح أن تخطط له كمسار مدته **18–24 شهراً**، مع إمكانية تمديده إذا أردت الوصول إلى عمق أكبر في CUDA وInference Engines.

سأفترض مبدئياً أنك تستطيع تخصيص 10–12 ساعة أسبوعياً. هذا افتراض تنظيمي، وليس شرطاً لإنجاز المسار.

**توزيع وقت الدراسة الأسبوعي**

**المجموع**

# **12 ساعة**

الكتب والفهم النظري

4 ساعات

البرمجة والتطبيق

4 ساعات

المشاريع والتجارب

3 ساعات

المراجعة والتوثيق

ساعة

لا أنصحك بأن تشاهد كورساً كاملاً ثم تنتقل إلى مشروع. الأفضل أن تدرس مفهوماً، وتختبره، وتبني شيئاً باستخدامه، ثم تعود للمراجع عندما تحتاج إلى تعميق فهمك.

وبما أنك تفضل المشاريع والكتب والتوثيق الرسمي، سنستخدم ثلاثة أنواع من المصادر:

1. **Textbooks:** للفهم العميق والتأسيس.
2. **Official Documentation:** لفهم السلوك الحقيقي والتفاصيل التنفيذية.
3. **Source Code & Projects:** لمعرفة كيف يحل المهندسون المشاكل في الأنظمة الحقيقية.

# **ثانياً: المنهج الدراسي التفصيلي**

سأقسم المنهج إلى 8 مراحل. كل مرحلة لها:

- المتطلبات السابقة.
- المفاهيم التي يجب فهمها.
- الكتب والمراجع.
- التطبيقات والمشاريع.
- مخرجات يمكن اختبارها قبل الانتقال.

## **المرحلة 0 — تجهيز الأساس البرمجي**



بوابة الدخول

&#x20;3–4 أسابيع



قبل أن تدخل Systems Programming، تحتاج أن تكون مرتاحاً في التعامل مع C وبيئة بناء البرامج.

لا نحتاج إلى إعادة دراسة البرمجة من الصفر، لكن نريد سد الفجوات التي ستظهر عندما تبدأ التعامل مع الذاكرة والنظام.

**الموضوعات**

| الموضوع        | ما يجب أن تتقنه                               |
| -------------- | --------------------------------------------- |
| C Fundamentals | Pointers، Arrays، Structs، Functions          |
| Memory         | Stack، Heap، Allocation، Deallocation         |
| Compilation    | Preprocessing، Compilation، Assembly، Linking |
| Debugging      | GDB، Breakpoints، Stack Traces                |
| Build Systems  | Make، CMake                                   |
| Git            | Branches، Commits، Debugging Changes          |
| Testing        | Unit Tests، Assertions، Sanitizers            |

**المراجع**

- [C Language Reference](https://en.cppreference.com/w/c?utm_source=chatgpt.com).
- [GCC Documentation](https://gcc.gnu.org/onlinedocs/?utm_source=chatgpt.com).
- [CMake Documentation](https://cmake.org/cmake/help/latest/?utm_source=chatgpt.com).
- [GDB Documentation](https://sourceware.org/gdb/documentation/?utm_source=chatgpt.com).

**المشروع: C Development Toolkit**

أنشئ مشروع C يحتوي على:

1. Dynamic Array.
2. Linked List.
3. Hash Table.
4. File Reader.
5. Memory Allocation Wrapper.
6. Test Suite.
7. Makefile أو CMake.

لا نريد مجرد تنفيذ Data Structures؛ نريد التعامل مع الذاكرة، وفهم أخطاء مثل Buffer Overflow وMemory Leak.

**معيار الانتقال**

تستطيع كتابة برنامج C متوسط الحجم، وتقسيمه إلى ملفات وموديولات، وبناؤه باستخدام CMake، وتتبع أخطائه باستخدام GDB وAddressSanitizer، وفهم دورة حياة الذاكرة التي يستخدمها.

## **المرحلة 1 — Computer Systems & Computer Architecture**



أساس جوهري

&#x20;8–10 أسابيع



هذه من أهم المراحل في التخصص كله.

قبل أن تدرس كيف يدير Linux الذاكرة، يجب أن تفهم ماذا تعني الذاكرة أصلاً، وكيف ينفذ المعالج التعليمات.

**الموضوعات**

[Central Processing Unit (CPU) Study Guide — OCR GCSE | Ma...](https://images.openai.com/static-rsc-4/kQPy2qs0txvmwQeXuNaO-M_D5M5ip_g_JbthO8G1cMuFgGm3rYedJcfZ_4LhVh6J052BfIOuYRcxCai-ozk15LvCKPSDaxNWtorsLghjbosruuzPuSivjQsHhaWxpjk_2Fx-GVpGso0KVx8vhx8ldReEBAUpgCKml3x4abnhE6E?purpose=inline)

**1. CPU Architecture**

- CPU Registers.
- Instruction Set Architecture.
- Fetch / Decode / Execute.
- Machine Instructions.
- Assembly Basics.

[Understanding How Computers Actually Work - DEV Community](https://images.openai.com/static-rsc-4/lsG9ffexUDgyRGVDxSqNTnyWRp0Wt8sDLuj6SYpaaD6hhu_im6HewEPg8PnTJyWuTbMLqWbXaEot-KPWPZ2BvdHYER2coW9opYDh8KbQgkbYbjdSotEXyPSHK-QagUyNHYbV5KmQvF5COjH4qNd1hLahfnAtAZI9XKoMR65ZSUQ?purpose=inline)

**2. Memory Hierarchy**

- Registers.
- CPU Cache: L1 / L2 / L3.
- RAM.
- Virtual Memory.
- Cache Locality.
- Memory Latency وBandwidth.

[The Linux Concept Journey — GNU Toolchain | by Shlomi Boutnaru, Ph.D. | Medium](https://images.openai.com/static-rsc-4/tBzycHG5m4UJ3wjV-XPjdOoEpWO76e3NzCwXpKKzuyYlWrJprx22Lx5zL2DlzCXvOPfSzASKyy4CwWIgYs4gsL8WzMNVvEa1V9btDFV5E2HT9GyMwY7ONp2mOzN8MJxdZEIGPEYbUmcimPer0_rfw7oJQdaM136XJ4L57nVrTfo?purpose=inline)

**3. Program Execution**

- Compiler.
- Assembler.
- Linker.
- Object Files.
- ELF.
- Dynamic Libraries.
- Stack Frames.

[Maximizing Performance in Embedded Linux with Cache-Aware Programming | by Wadix Technologies | Embedded Systems Technologies | Medium](https://images.openai.com/static-rsc-4/QwXlB9zs3wfU_mwuhUsJ68RzJKq3mCwNSs4PFsS6dQ2lCeP9lL0qPw5REPybx-mgQfkocXOPANLLIFzyTvzR05CWwoqQi2lkybpWO5TxWc3i020Hm8rc3palHIe3RaIRPH9-rJTRNzO-sX_zuFf_0PsnOWJz8OUVccm_77spz78?purpose=inline)

**4. Performance Fundamentals**

- Cache Misses.
- Branch Prediction.
- Instruction-Level Parallelism.
- Data Locality.
- CPU-bound vs Memory-bound.

**الكتاب الرئيسي:**

[Computer Systems: A Programmer's Perspective 3rd Edition 非扫描版 - 经管之家](https://images.openai.com/static-rsc-4/ljWgBdhTAOUwfL1ADQGs3oQBLzZAv_oRadU7A84is2XEs_r7uwvKoiUviUB5EZMi39SjmXyal98G_i10mP6kT4cAhzcyysk1NjtM4JdR8-SSt1oWKLaO_97DWFx_soYkMazH3Tcskz6GdHeNauf8-oLcLrXOWUONjL3BDbz3Aw0?purpose=inline)

**Computer Systems: A Programmer's Perspective**

Bryant & O'Hallaron

هذا الكتاب سيكون مرجعك الأساسي في هذه المرحلة، وربما تعود إليه لاحقاً.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://csapp.cs.cmu.edu\&sz=32)

csapp.cs.cmu.edu+1



ادرس منه بالترتيب:

- Chapter 1: A Tour of Computer Systems.
- Chapter 2: Representing and Manipulating Information.
- Chapter 3: Machine-Level Representation.
- Chapter 4: Processor Architecture.
- Chapter 5: Optimizing Program Performance.
- Chapter 6: Memory Hierarchy.
- Chapter 7: Linking.
- Chapter 9: Virtual Memory.

**ملاحظة مهمة لجهازك:** الطبعة الثالثة من CS:APP تركز على x86-64، بينما معالج Apple Silicon يستخدم ARM64. تستطيع دراسة المفاهيم على الماك، لكن تطبيق Assembly ومختبرات الكتاب التي تعتمد على x86-64 يحتاجان بيئة x86-64 مناسبة، مثل Linux VM على جهاز سحابي. لا تخلط بين اختلاف ISA واختلاف المفاهيم المعمارية.

**المشاريع**

**Project 1 — Program Execution Explorer**

اكتب برنامج C بسيطاً، ثم حلل رحلته:

- افحص الـ Assembly الناتج.
- افحص الـ Object File.
- افحص الـ ELF عند العمل على Linux.
- افحص Stack وHeap.
- افحص المكتبات المرتبطة بالبرنامج.

**Project 2 — Cache Performance Lab**

اكتب برامج تنفذ عمليات على مصفوفات كبيرة بطرق مختلفة، وقارن أداء:

- Sequential Access.
- Random Access.
- Row-major vs Column-major.
- Different Data Structures.

استخدم Benchmarking وProfiler لتفسير النتائج، وليس فقط قياس الزمن.

**مخرجات المرحلة**

تستطيع تفسير ما يحدث عندما تشغّل برنامج C من لحظة تشغيله حتى تنفيذ تعليماته، وتفهم تأثير الذاكرة والكاش والمعالج على أدائه.

## **المرحلة 2 — Operating Systems & Linux Internals**



أساس جوهري

&#x20;10–12 أسبوعاً



هنا تبدأ Systems Programming الفعلية.

أريدك أن تفهم نظام التشغيل من جهتين:

1. النظريات: كيف يصمم نظام التشغيل آليات إدارة الموارد؟
2. التطبيق: كيف يستخدم البرنامج هذه الآليات من خلال Linux APIs؟

### **الجزء الأول: Operating Systems**

**الموضوعات**

| المجال      | التفاصيل                              |
| ----------- | ------------------------------------- |
| Processes   | Creation، States، Context Switching   |
| Scheduling  | CPU Scheduling، Scheduling Policies   |
| Memory      | Virtual Memory، Paging، Page Tables   |
| Threads     | Thread Lifecycle، Synchronization     |
| Concurrency | Mutex، Semaphore، Condition Variables |
| Persistence | Filesystems، I/O، Storage             |
| Deadlocks   | Prevention، Detection، Recovery       |

**الكتاب الرئيسي:**

[Operating Systems: Three Easy Pieces](https://images.openai.com/static-rsc-4/Cl_YdedpQ_GntLrRVelbWQjwmR4yTRM2S0GKDQpkXe7sDyk-TetfJX70RHdLfN51BMpnSIkfFZHVvrq-rY6U8-H9Tg_YW8a8ssi6PryqNketQIUS9Qcr7gTPVQq7ZdLeevYlMvqGRsUogmnptE0xsueo3iKErTQbYLa4rnc6dY4?purpose=inline)

**Operating Systems: Three Easy Pieces**

Remzi & Andrea Arpaci-Dusseau

كتاب مجاني رسمياً، ومناسب جداً للتعلم العميق مع تجارب ومختبرات.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://research.cs.wisc.edu\&sz=32)

research.cs.wisc.edu+1



[الكتاب والمختبرات](https://pages.cs.wisc.edu/~remzi/OSTEP/?utm_source=chatgpt.com)

ادرس الأقسام الثلاثة:

- Virtualization.
- Concurrency.
- Persistence.

لا تقرأ الكتاب كأنه رواية. حل المسائل والـ Simulators الموجودة معه.

### **الجزء الثاني: Linux System Interfaces**

بعد أن تفهم النظرية، انتقل إلى كيفية استخدام Linux لها.

**الموضوعات**

- `fork()` و`exec()`.
- `wait()` و`waitpid()`.
- `open()` و`read()` و`write()`.
- `mmap()` و`munmap()`.
- `pipe()` و`dup2()`.
- `pthread_create()`.
- Signals.
- Shared Memory.
- Semaphores.
- Unix Domain Sockets.
- `/proc`.

**المرجع الرئيسي:**

[The Linux Programming Interface by Michael Kerrisk - Penguin Books New Zealand](https://images.openai.com/static-rsc-4/Z7-zs2r7kqGOsGAqEoCuKLqPMEtjDGUADSl0J6pYiroywYlnrLb9zgfSXMq88F0CuKdjfBvyj91AwfqN4-Dy7d2_2iNtziFtuyC280Gyt_B4ntJmuJIkU2LCmSxCSIOBJulaHaDwTSr4-hQtUIVV_ihNuUIyXWBxRpJRlIxjzM0?purpose=inline)

**The Linux Programming Interface**

Michael Kerrisk

هذا المرجع مهم جداً في هذا المسار. لا تحتاج قراءة صفحاته الـ1552 كاملة من البداية للنهاية؛ استخدم فصوله حسب الموضوع.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://www.kerrisk.com\&sz=32)

kerrisk.com+1



[الموقع الرسمي ومصادر الكتاب](https://man7.org/tlpi/?utm_source=chatgpt.com)

**المشاريع**

**Project 1 — تطوير Shell الذي بدأت به**

لا تبدأ Shell جديداً. طور مشروعك الحالي.

أضف:

- Process Creation.
- Command Execution.
- Pipes.
- Input/Output Redirection.
- Signals.
- Background Processes.
- Job Control.

الهدف أن تفهم كيف يتعاون Shell مع Kernel.

**Project 2 — Process Manager**

برنامج يعرض العمليات النشطة ويتعامل معها.

- PID وPPID.
- Process States.
- CPU وMemory Usage.
- إرسال Signals.
- عرض Process Tree.

استخدم `/proc` وواجهات Linux المناسبة.

**Project 3 — Memory Allocator**

اكتب Allocator مبسطاً بلغة C.

- Allocate / Free.
- Free Lists.
- Memory Blocks.
- Fragmentation.
- Allocation Strategies.

لا تحاول إعادة بناء `malloc` بالكامل؛ الهدف فهم المبادئ.

**مراجع رسمية مكملة**

- [Linux Kernel Documentation](https://www.kernel.org/doc/html/latest/?utm_source=chatgpt.com).
- [Linux man-pages](https://man7.org/linux/man-pages/?utm_source=chatgpt.com).
- [fork System Call](https://man7.org/linux/man-pages/man2/fork.2.html?utm_source=chatgpt.com).
- [mmap System Call](https://man7.org/linux/man-pages/man2/mmap.2.html?utm_source=chatgpt.com).

ملاحظة: وثائق Kernel ليست كتاباً للمبتدئين. استخدمها بعد فهم المفهوم من OSTEP وTLPI. حتى وثائق Memory Management نفسها توضح أن بعض أجزائها لا تزال غير مكتملة.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://www.kernel.org\&sz=32)

The Linux Kernel documentation



**مخرجات المرحلة**

تستطيع كتابة برنامج C يستخدم Linux System Calls، وتفهم إنشاء العمليات والخيوط وإدارة الذاكرة والتزامن والملفات، وتستطيع تشخيص مشاكلها.

## **المرحلة 3 — Advanced Systems Programming & Performance**



انتقال إلى المستوى المتقدم

&#x20;8–10 أسابيع



هنا لا نكتفي بأن يعمل البرنامج؛ نريد أن نفهم كيف نجعله سريعاً وقابلاً للتوسع.

**الموضوعات**

1. Advanced Memory Management.
2. Multithreading.
3. Locks & Lock-free Concepts.
4. Atomic Operations.
5. Thread Pools.
6. Non-blocking I/O.
7. Event-driven Architecture.
8. epoll.
9. Performance Profiling.
10. Cache-aware Programming.

**الكتاب الرئيسي:**

[Systems Performance (2nd ed.) by Brendan Gregg (ebook)](https://images.openai.com/static-rsc-4/1qEwIYrFd6Yra25Kujzaoy1RFaeBL1ML-f2AT_E_e52igOV6MU_Ja-T2Krlfd5C9s04ADdaepRJ8szEOVnhOR-NYiKvi5dfjlr6VYRYLZzaj5M9bJTRRKvKfvfo88jZSWnA2Av0exU0fe-RSe57-kABabElHO2korrPvZLh4fq4?purpose=inline)

**Systems Performance**

Brendan Gregg

مرجع مهم لتعلم تحليل أداء الأنظمة واكتشاف الاختناقات. [صفحة الكتاب](https://www.brendangregg.com/systems-performance-2nd-edition-book.html?utm_source=chatgpt.com).

**الأدوات**

- GDB.
- Valgrind.
- `perf`.
- `strace`.
- `ltrace`.
- `htop`.
- `bpftrace` (مقدمة).
- Google Benchmark.

**المشاريع**

**Project 1 — Multithreaded HTTP Server**

باستخدام C أو C++.

- TCP Sockets.
- Thread Pool.
- Request Handling.
- Non-blocking I/O.
- epoll على Linux.
- Connection Management.

**Project 2 — Benchmarking Suite**

اختبر برنامجك تحت أحمال مختلفة.

قس:

- Requests per Second.
- P50 / P95 / P99 Latency.
- CPU Utilization.
- Memory Usage.
- Context Switches.

ثم جرب تغيير Thread Pool Size وآلية التعامل مع الاتصالات، وقارن النتائج.

**مخرجات المرحلة**

تستطيع بناء برنامج متعدد الخيوط، وتحليل الأداء، وتفسير الاختناقات بدلاً من التخمين.

## **المرحلة 4 — C++ Systems Engineering**

8–10 أسابيع

أنت لا تحتاج C++ فقط لأنك تريد برمجة منخفضة المستوى؛ تحتاجها لأنها لغة رئيسية في بناء كثير من الأنظمة عالية الأداء، بما فيها أجزاء من أنظمة تشغيل النماذج ومحركات التنفيذ.

هنا ننتقل من C إلى C++ بصورة منظمة.

**الموضوعات**

| الموضوع          | لماذا تحتاجه؟                  |
| ---------------- | ------------------------------ |
| RAII             | إدارة الموارد بأمان            |
| Smart Pointers   | التحكم في ملكية الذاكرة        |
| Move Semantics   | تجنب النسخ غير الضروري         |
| Templates        | بناء مكونات عامة وعالية الأداء |
| STL              | Containers وAlgorithms         |
| Multithreading   | Concurrency                    |
| Atomics          | العمليات المتزامنة             |
| Memory Alignment | التعامل مع الذاكرة بكفاءة      |
| CMake            | بناء مشاريع كبيرة              |
| Profiling        | تحليل الأداء                   |

**المراجع**

- [ISO C++ Getting Started](https://isocpp.org/get-started?utm_source=chatgpt.com).
- [cppreference](https://en.cppreference.com/w/cpp?utm_source=chatgpt.com).
- [Clang Documentation](https://clang.llvm.org/docs/?utm_source=chatgpt.com).

**الكتاب المقترح:** *A Tour of C++* لـ Bjarne Stroustrup، ثم *C++ Concurrency in Action* لـ Anthony Williams عند دخول التزامن المتقدم.

**المشاريع**

- Thread Pool Library.
- High-performance Key-Value Store.
- Memory Pool.
- C++ Networking Library.

وأريدك أن تكتب اختبارات أداء لهذه المشاريع، وتقارن بين أكثر من تصميم، وتوثق أسباب اختيارك.

**مخرجات المرحلة**

تستطيع بناء مكتبة C++ منظمة وقابلة لإعادة الاستخدام، تفهم إدارة الموارد والتزامن، وتستطيع ربطها ببرنامج Python عند الحاجة.

## **المرحلة 5 — GPU Architecture & CUDA Programming**



بداية AI Systems المتخصص

&#x20;10–12 أسبوعاً



هذه أول مرحلة تنتقل فيها بصورة مباشرة من Systems Programming إلى AI Infrastructure.

قبل أن تفتح CUDA، يجب أن تفهم أن GPU ليست مجرد CPU أسرع.

طريقة تنفيذ العمليات، والذاكرة، والتوازي، وإدارة البيانات تختلف بصورة مهمة.

**المتطلبات السابقة**

- C/C++ جيد.
- Pointers وMemory Management.
- Threads وConcurrency.
- أساسيات Linear Algebra.
- فهم Matrix Multiplication.
- Floating Point Representation.

### **الموضوعات**

[CUDA — High-Level Guide. GPU Programming In A Nutshell | by Ozgun Ozerk | Medium](https://images.openai.com/static-rsc-4/D_PK6e5OpEcjZuTceyQ75pkmfhhhdVHlt8szf1-VxgblPGgPkVKOlCZXuEf4XQdFBKRCxYXt_3N_oktm44esnuqP1iSym_NE_VB6Ysx_ESGr6v8Ys9oYO8HXNN41lujDubPmLSFqhJrhD6Xyyl_dyI5vIqyin6I81BxfhHGkKXo?purpose=inline)

**GPU Architecture**

- Streaming Multiprocessors.
- CUDA Cores.
- Warps.
- Threads وBlocks.
- Occupancy.

[Jerarquía de memoria png imágenes | PNGWing](https://images.openai.com/static-rsc-4/7sxWom_m0v_tpryk-uxKN2i_ZCWcFwqb7COu4FYw9PfuLikafy32pV690D0ARESZ6vSCjTM7T8mL-_BZX0Bbv99IkMIIssQfpzbdqpFftYF5GItCejRK5T0l2wsFqKoVtGQYMleSl9s9PiGSvU7pxKLB0gP62OORjbndzf6yt2Y?purpose=inline)

**GPU Memory Hierarchy**

- Registers.
- Shared Memory.
- Global Memory.
- Cache.
- Memory Coalescing.
- Host-to-Device Transfer.

[Matrix Multiplication | Zobin](https://images.openai.com/static-rsc-4/4dUrqJ1HtpmPlQvzV50OqFD_iXEUFSk8YUbsxV8VhFrZA--6CdaT0mxFJg9MHpmaXEOR-NdInMpU9w8gudicaxO1Ejk8J5kAzCHv5vfsfUoHe-Bi1ILnlKD6UKPij-nqtOqr0dakPZQI6p70gX2u2pRGFGNVIAlN8yA7nGYuxFo?purpose=inline)

**Parallel Programming**

- CUDA Kernels.
- Thread Blocks.
- Grid Dimensions.
- Synchronization.
- Reduction.
- Matrix Multiplication.

**المرجع الأساسي**

[Programming Massively Parallel Processors 	- 	Edition 	5 	- 	By Wen-mei W. Hwu, David B. Kirk and Izzat El Hajj                     Elsevier Educate](https://images.openai.com/static-rsc-4/fECoSFySyDQ_V9NwsVo1n6vDJxQxiAjr029GKokWwE3i6O8eOkTD9ChGshLnjpzCCJ0So2cCTbwqzXRWYn5xrarpCx9-j_l32l5XfAVZ-0AGQx31vEMGrms7GbGpJUZDGgqp6leIchzOAvzxFJeTey_vlv9zo6csFe0k5Ecq9dI?purpose=inline)

**Programming Massively Parallel Processors**

مرجع لفهم GPU Parallel Programming.

اقرأ بالتوازي مع [NVIDIA CUDA Programming Guide](https://docs.nvidia.com/cuda/cuda-programming-guide/?utm_source=chatgpt.com). الدليل الرسمي يغطي نموذج البرمجة، الذاكرة، والتنفيذ المتقدم.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://docs.nvidia.com\&sz=32)

CUDA Programming Guide



**المشاريع**

1. Vector Addition Kernel.
2. Matrix Multiplication Kernel.
3. Parallel Reduction.
4. Softmax Kernel.
5. Layer Normalization Kernel.
6. مقارنة CPU وGPU على عمليات مختلفة.

لا تبدأ بكتابة Transformer كامل باستخدام CUDA. ابدأ بالعمليات الصغيرة، وافهم الذاكرة والتوازي والقياس.

**مخرجات المرحلة**

تستطيع كتابة CUDA Kernels، وفهم كيفية توزيع العمل على GPU، وتحليل استهلاك الذاكرة والأداء.

**شرط الجهاز:** الماك مفيد لتعلم C++ ومفاهيم GPU العامة، لكنه لا يشغّل CUDA على Apple GPU. ستحتاج إلى NVIDIA GPU سحابي عند تنفيذ تجارب CUDA الحقيقية. لا تحتاج شراء جهاز GPU خاص بك.

## **المرحلة 6 — Deep Learning Execution & LLM Inference Fundamentals**



الانتقال إلى Inference Engineering

&#x20;8–10 أسابيع



هذه المرحلة تربط معرفتك السابقة بالـ Deep Learning مع ما تعلمته عن الأنظمة والـ GPU.

أنت لا تحتاج إلى إعادة دراسة Machine Learning أو Deep Learning من البداية. تحتاج أن تفهم كيف يتحول النموذج الذي تعرفه إلى عملية تنفيذ فعلية على CPU أو GPU.

### **الجزء الأول: كيف يعمل Inference؟**

ادرس دورة تنفيذ نموذج Transformer:

**LLM Inference Lifecycle**

**Input Text**

User Prompt

**Tokenization**

Text → Token IDs

**Prefill**

Process input tokens · Compute KV Cache

**Decode**

Generate tokens autoregressively · Reuse KV Cache

**Output**

Generated Tokens → Text

**الموضوعات**

- Transformer Inference.
- Attention Computation.
- Prefill vs Decode.
- KV Cache.
- Autoregressive Generation.
- Sampling Algorithms.
- Quantization: FP16، BF16، INT8، INT4.
- Memory Bandwidth.
- Compute-bound vs Memory-bound.
- Batch Processing.

### **الجزء الثاني: PyTorch Internals**

تعرف على:

- Tensor Operations.
- Tensor Memory Layout.
- CUDA Streams.
- Synchronization.
- Autograd مقابل Inference.
- `torch.no_grad()` و`torch.inference_mode()`.
- C++ Extensions.

**المراجع**

- [PyTorch CUDA Semantics](https://docs.pytorch.org/docs/stable/notes/cuda.html?utm_source=chatgpt.com).
- [PyTorch C++ Frontend](https://docs.pytorch.org/cppdocs/?utm_source=chatgpt.com).
- [Attention Is All You Need](https://arxiv.org/abs/1706.03762?utm_source=chatgpt.com).
- [FlashAttention-2](https://arxiv.org/abs/2307.08691?utm_source=chatgpt.com).

الـ C++ Frontend في PyTorch مهم كمرجع لفهم الربط بين C++ وعمليات Tensor، لكن لا تفترض أن نقل كود Python إلى C++ يجعله أسرع تلقائياً؛ PyTorch ينفذ كثيراً من العمليات الثقيلة أصلاً في C++ وCUDA.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://docs.pytorch.org\&sz=32)

PyTorch main documentation



### **المشروع: Build an Inference Benchmarking Tool**

ابنِ أداة تقارن تشغيل نموذج عبر إعدادات مختلفة.

مثلاً:

| التجربة                  | ما تقيسه            |
| ------------------------ | ------------------- |
| Batch Size 1             | Latency             |
| Batch Size 4             | Throughput          |
| Batch Size 8             | GPU Utilization     |
| FP16 vs BF16             | Performance وMemory |
| Different Prompt Lengths | Prefill Latency     |
| Different Output Lengths | Decode Performance  |

أخرج تقريراً يوضح:

- Time to First Token (TTFT).
- Time Per Output Token (TPOT).
- Tokens per Second.
- Requests per Second.
- Peak GPU Memory.

**مخرجات المرحلة**

تستطيع تفسير ما يحدث أثناء Inference، وتفرق بين تكلفة Prefill وDecode، وتعرف كيف تؤثر الذاكرة وحجم Batch على أداء النموذج.

## **المرحلة 7 — LLM Inference Engine Architecture**



التخصص الرئيسي

&#x20;10–12 أسبوعاً



هنا تبدأ دراسة الأنظمة التي تستخدمها شركات AI Infrastructure فعلياً.

أريدك أن تنتقل من مجرد تشغيل نموذج إلى فهم محرك التشغيل نفسه.

### **الموضوعات الأساسية**

**1. Memory Management for LLMs**

- KV Cache Allocation.
- KV Cache Eviction.
- PagedAttention.
- Memory Fragmentation.
- Prefix Caching.
- Block Management.

**2. Scheduling**

- Request Scheduling.
- Continuous Batching.
- Dynamic Batching.
- Chunked Prefill.
- Request Prioritization.

**3. Execution Engine**

- Model Runner.
- Token Generation.
- CUDA Graphs.
- Attention Kernels.
- Model Execution Pipeline.

**4. Serving Architecture**

- API Server.
- Engine Core.
- GPU Workers.
- Request Queues.
- Streaming Responses.
- Cancellation.
- Backpressure.

### **المرجع التطبيقي الأساسي: vLLM**

[Ollama vs vLLM: A Comprehensive Guide to Local LLM Serving | by Mustafa Genc | Feb, 2026 | Medium](https://images.openai.com/static-rsc-4/AEzYgZrtwKLxf_M9_Z4Cg2z5_P8kWauAxXzasVQmMq1DK1O7WsFshDS9wyFaijD5opAWtNubHJus7WSBs5oraDVt5D_WrpgYlhaZQQ7GrdK31CT5IhtpNKwB0HxIDeoTnC9D8wneMieTWUTjABwsGqN844qCmgJbA3OmM_-hseM?purpose=inline)

**vLLM**

أريدك أن تتعامل معه كدراسة هندسية، وليس مجرد مكتبة تثبتها وتستخدمها.

وثائقه تشرح PagedAttention وContinuous Batching وKV Cache وطرق توزيع عمليات Inference.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://docs.vllm.ai\&sz=32)

docs.vllm.ai+1



[Documentation](https://docs.vllm.ai/en/stable/?utm_source=chatgpt.com) · [Source Code](https://github.com/vllm-project/vllm?utm_source=chatgpt.com)

### **كيف تدرس vLLM؟**

لا تفتح آلاف الأسطر من الكود وتحاول فهمها دفعة واحدة.

استخدم هذا الترتيب:

1. اقرأ Architecture Overview.
2. افهم API Server.
3. افهم Engine Core.
4. افهم GPU Workers.
5. افهم Model Runner.
6. ادرس KV Cache Management.
7. تتبع رحلة Request واحدة داخل النظام.
8. اقرأ الكود المرتبط بكل جزء.

وثائق vLLM الحالية تصف معمارية متعددة العمليات، تفصل بين API Server وEngine Core وGPU Workers؛ وهذه نقطة ممتازة لدراسة العلاقة بين Systems Programming وInference Engineering.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://docs.vllm.ai\&sz=32)

vLLM



### **المشروع: Mini Inference Engine**

هنا أريدك أن تبني محركاً مبسطاً، لا أن تكتب Transformer من الصفر بالضرورة.

ابدأ باستخدام نموذج صغير مفتوح المصدر ومكتبة Tensor Execution موجودة.

ثم ابنِ طبقاتك بنفسك:

**تصميم المشروع**

**Client Requests**

**Request Manager**

Queue · Validation · Cancellation

**Scheduler**

Batching · Request Scheduling

**Inference Engine**

Prefill · Decode · KV Cache

**Execution Backend**

PyTorch / CUDA · GPU Memory

نفذ المشروع تدريجياً:

- أولاً طلب واحد.
- ثم عدة طلبات متزامنة.
- ثم Request Queue.
- ثم Dynamic Batching.
- ثم KV Cache Manager.
- ثم قياس الأداء.

**مخرجات المرحلة:** تستطيع تفسير بنية Inference Engine، وتكتب محركاً تعليمياً يحتوي على إدارة طلبات وجدولة وتنفيذ وقياسات أداء.

## **المرحلة 8 — Advanced AI Inference & Optimization**



مستوى التخصص

&#x20;12–16 أسبوعاً



هذه المرحلة ستحدد مدى عمق تخصصك.

لن نكتفي باستخدام vLLM، بل نبدأ بدراسة تقنيات التحسين الموجودة في محركات Inference الحديثة.

### **الموضوعات**

| المجال                 | ما تتعلمه                          |
| ---------------------- | ---------------------------------- |
| Attention Optimization | FlashAttention، FlashInfer         |
| Memory Optimization    | Paged KV Cache، Prefix Caching     |
| Quantization           | AWQ، GPTQ، FP8                     |
| GPU Execution          | CUDA Graphs، Kernel Fusion         |
| Speculative Decoding   | Draft Models، Verification         |
| Scheduling             | Chunked Prefill، Advanced Batching |
| Distributed Inference  | Tensor Parallelism                 |
| Profiling              | Nsight Systems، Nsight Compute     |

**المراجع الرسمية**

- [NVIDIA Nsight Systems](https://docs.nvidia.com/nsight-systems/?utm_source=chatgpt.com).
- [NVIDIA Nsight Compute](https://docs.nvidia.com/nsight-compute/?utm_source=chatgpt.com).
- [vLLM Developer Documentation](https://docs.vllm.ai/en/stable/?utm_source=chatgpt.com).
- [CUDA Documentation](https://docs.nvidia.com/cuda/?utm_source=chatgpt.com).

### **المشاريع**

**Project 1 — KV Cache Manager**

ابنِ نظاماً مستقلاً لإدارة KV Cache.

- تقسيم الذاكرة إلى Blocks.
- تخصيص Blocks للطلبات.
- تحرير الذاكرة بعد انتهاء الطلب.
- التعامل مع الطلبات ذات الأطوال المختلفة.
- قياس Fragmentation وMemory Utilization.

**Project 2 — CUDA Kernel Optimization**

اختر عملية واحدة من عمليات Transformer، مثل:

- Softmax.
- Layer Normalization.
- Matrix Multiplication.
- Attention.

اكتب Kernel مبسطاً ثم قارن أداءه بتنفيذ مرجعي. استخدم Profiling لتحديد أسباب الفروقات.

**Project 3 — Inference Optimization Report**

خذ نموذجاً واحداً وثبت بيئة الاختبار، ثم قارن:

- Baseline Inference.
- Batching.
- Quantization.
- KV Cache Optimization.
- Kernel Optimization.

لا تكتفِ بقول إن النسخة الثانية أسرع؛ أريد تفسيراً هندسياً للسبب، مع نتائج قابلة لإعادة الإنتاج.

**مخرجات المرحلة**

تستطيع تحليل محركات Inference، وتفهم خيارات تحسين الذاكرة والحساب والجدولة، وتنفذ تحسيناً واحداً على الأقل وتثبت أثره بقياسات موثوقة.

# **ثالثاً: مشروع التخرج — نظام يجمع التخصص كاملاً**

بعد هذه المراحل، أريد مشروعاً واحداً كبيراً بدلاً من 10 مشاريع منفصلة غير مترابطة.

Capstone Project

# **Build Your Own LLM Runtime & Serving System**

[Hosting LLMs — From Fundamentals to Scaled Production (with Hands-On Tutorial) | by Shawn | Medium](https://images.openai.com/static-rsc-4/b57oA8XCAza9h65hP5ZLBOcjLvKLb6BeO3SupR7UbWk6fS0PHjIOTLnNwMty5TjbbtCjArcuHvfjlgRFfy0_kwii8BJQjlQNHfbpSru2quqn-jPuIKDPr1CXcATvxamE8O38zNZkDlE7TOW1Loy4__wSWsPfuuhtMH2UNFZtm_o?purpose=inline)

[medium.com](https://medium.com/%40xiaxiami/hosting-llms-from-fundamentals-to-scaled-production-with-hands-on-tutorial-6598d16810e0?utm_source=chatgpt.com)

**الهدف:** بناء نظام تشغيل وتقديم نماذج لغوية، مع تصميم وإدارة أجزاء من البنية الداخلية بنفسك.

**المكونات:**

1. **Runtime:** مسؤول عن تنفيذ النموذج.
2. **Memory Manager:** إدارة KV Cache.
3. **Scheduler:** تنظيم الطلبات.
4. **Execution Backend:** PyTorch وCUDA.
5. **Serving Layer:** استقبال الطلبات وبث الإجابات.
6. **Monitoring:** قياس الموارد والأداء.
7. **Benchmarking:** مقارنة نظامك مع vLLM.
8. **Testing:** اختبار الصحة والأداء والتزامن.

**اللغات:**

- C++ للأجزاء التي تحتاج أداء وتحكماً أكبر.
- CUDA للعمليات التي تنفذ على NVIDIA GPU.
- Python للتكامل مع النماذج والاختبارات.
- Linux لتشغيل النظام وتحليله.

لا يشترط أن تكتب كل مكونات المشروع من الصفر. بالعكس، المهندس الجيد يعرف ما الذي ينبغي أن يبنيه بنفسه وما الذي ينبغي أن يستخدم له مكتبة جاهزة.

مثلاً، يمكنك استخدام PyTorch لتنفيذ العمليات الرياضية، ثم بناء Scheduler وKV Cache Manager وServing Layer بنفسك. وبعدها تتوسع تدريجياً نحو تنفيذ Kernels خاصة بك.

# **رابعاً: كيف تستخدم الماك بوك طوال هذا المسار؟**

أقترح أن تكون بيئتك ثلاثية:

[Josean Martinez](https://images.openai.com/static-rsc-4/XNRYv-B6-IBeQnI0DCFwFcl8ACUkYUiIBP-ombfRGrwULa7DvAa0k-VlsNoF4sjNOOslDgsI6kogUowWaeHEYjQJGO4Ad0bPvsSZkfXIPNQwo77kM65D0EOECiQB3hUcDczVgtCmxim7_F5scL3VTMHwceUv98G1kz82f4t4wxY?purpose=inline)

**1. macOS — بيئة التطوير الرئيسية**

- VS Code.
- C/C++ وPython.
- CMake.
- Git.
- GDB/LLDB.
- كتابة واختبار البرامج.

[Creating a Professional Home Lab Setup -Part 3: Virtual Machine Management | by Tadaweb | Tadaweb | Medium](https://images.openai.com/static-rsc-4/NVnEV_kQyg3wxp29_OEEORxh1SqAMTsW7kfyBVRDu5UnFjNeLpPDeB7uLTPmNG42ZmEPZcAqEoh5C7kosDNAo2XMD-luhYSBbHFS1JdP53KJ47jl3gvNZDdQnsCiJlrXnRpaP-knb_Xs8a9GiEPnzdFK2sCkQ9jgUWlAPjne_os?purpose=inline)

**2. Ubuntu Linux VM — مختبر الأنظمة**

استخدم UTM أو بيئة Linux افتراضية.

- Linux System Calls.
- Processes وThreads.
- `/proc`.
- `strace` و`perf`.
- Linux Networking.
- Linux-specific experiments.

ابدأ بـ Ubuntu Server، ويمكنك تشغيلها عبر SSH من الماك.

[95%对40%背后：GPT-6 Astra赢了机械臂测试，但赢得不太干净 - ic.work](https://images.openai.com/static-rsc-4/PgOKWUpRIzU6XSi16DwIyddAnQ05C6Dz6-mjYOdpqpS-uQVY06_aiGxkUr0imjEyJHlDXOYMAdzDwLbtC4-SJGzGU9vPuS0l5E4C5b-N3NTJoRyq-dFTrJkEwMkDwIQZWr8yrxqZ0eEwm_0Q_U7BeYLEgsSVZoPjOIVA8Frp1Ls?purpose=inline)

**3. NVIDIA GPU Cloud — مختبر الذكاء الاصطناعي**

استخدمه عندما تصل إلى CUDA وGPU Inference.

- CUDA Kernels.
- GPU Profiling.
- vLLM.
- KV Cache.
- Inference Benchmarking.

لا تستأجر GPU إلا عندما تحتاج إلى تجربة محددة، وأوقفه عند انتهاء التجربة لتتحكم بالتكلفة.

نقطة مهمة: لا تعتبر Docker بديلاً عن Linux VM عند دراسة Kernel Interfaces أو إدارة النظام. Docker مفيد لاحقاً لتغليف وتشغيل التطبيقات، أما تعلم النظام نفسه فيحتاج بيئة Linux حقيقية.

# **خامساً: كيف تعرف أنك تتقدم فعلاً؟**

لا أريد أن تقيس تقدمك بعدد الكتب التي أنهيتها أو الدورات التي شاهدتها.

سنستخدم مخرجات هندسية واضحة لكل مرحلة.

| المرحلة                   | الاختبار الذي يثبت إتقانها                          |
| ------------------------- | --------------------------------------------------- |
| 0. C Foundation           | كتابة برنامج C متعدد الملفات مع Debugging واختبارات |
| 1. Computer Systems       | تحليل تنفيذ برنامج وفهم الذاكرة وAssembly           |
| 2. OS & Linux             | بناء Shell والتعامل مع System Calls                 |
| 3. Advanced Systems       | بناء Server متعدد الخيوط وقياس أدائه                |
| 4. C++ Systems            | بناء Thread Pool وMemory Pool                       |
| 5. CUDA                   | كتابة Kernels وقياس أدائها                          |
| 6. Inference Fundamentals | قياس وتحليل Prefill وDecode                         |
| 7. Inference Engine       | بناء Mini Inference Engine                          |
| 8. Optimization           | تحسين جزء من المحرك وإثبات التحسن                   |

## **سجل الإنجازات الهندسي**

أقترح أن يكون لكل مشروع مستودع GitHub مستقل، وأن يحتوي على:

- `README.md`: المشكلة والحل والتصميم.
- `docs/architecture.md`: تصميم النظام.
- `docs/decisions.md`: القرارات الهندسية ولماذا اتخذتها.
- `benchmarks/`: نتائج قياس الأداء.
- `tests/`: الاختبارات.
- `src/`: الكود.

وأريد منك عادة مهمة: قبل أن تكتب المشروع، ارسم Architecture Diagram، وحدد المكونات، وكيف تتواصل، وما مسؤولية كل مكون.

هذا مهم لأنك لا تتعلم فقط كيف تكتب الكود، بل كيف تصمم نظاماً هندسياً.

# **سادساً: ما الذي لا أريدك أن تضيّع وقتك فيه الآن؟**

هذه نقطة مهمة حتى لا يتوسع المسار إلى درجة يصبح من المستحيل إنهاؤه.

| الموضوع                   | القرار                                                        |
| ------------------------- | ------------------------------------------------------------- |
| Linux Kernel Development  | اتركه للتخصص المتقدم لاحقاً                                   |
| Device Drivers            | غير مطلوب لمسار Inference                                     |
| Embedded Linux            | ليس ضمن أولوياتنا                                             |
| Kubernetes                | تعلم أساسياته بعد فهم Serving، وليس الآن                      |
| Rust                      | أجّله حتى تتقن أساسيات C/C++                                  |
| Go                        | ليس ضرورياً لهذا المسار                                       |
| Web Development           | احتفظ بمعرفتك السابقة ولا تتوسع فيه الآن                      |
| Building LLM from Scratch | ليس هدفنا الحالي                                              |
| Advanced Mathematics      | ركز على Linear Algebra وNumerical Computing المرتبطين بالأداء |

وأيضاً لا نحتاج أن ندرس كل ما في Linux Kernel أو كل ما في Computer Architecture. نريد عمقاً في الأشياء التي تخدم تخصصنا.

# **سابعاً: خريطة الكتب والمراجع التي ستعتمد عليها**

هذه قائمة مرجعية للمسار، وليست قائمة مطلوب منك شراء جميع كتبها الآن.

**Core Books — الكتب الأساسية**

[Computer Systems: A Programmer's Perspective (3rd Edition) - ISBN13:9780134092669 - 澜瑞外文-网上购买外文原版进口图书 LANREE](https://images.openai.com/static-rsc-4/nNQSwJGmi5taHAXfVaQQSDIYpxCQaNnp9kdNHc-q9kHg5BnP0N1HASLaVFwHTuDmHAzsa6W4mX1HVmO0hn_nUGhyjFlArQzrAZCMi569D8fVYzqZ4BlI_DcC-xwYqoIlILgZbs1TPxOIL86MIm0p37cOVSGoWiQH-rDALojRsBQ?purpose=inline)

**1. Computer Systems: A Programmer's Perspective**

Computer Architecture + Memory + Program Execution.

المرحلة 1

[The 10 Best Computer Operating Systems Theory Books of 2026 (Reviews) - FindThisBest](https://images.openai.com/static-rsc-4/4Qg-mqlY6v9MeBRiNSxPJ47DRK_Nc2l2z9iqCyiHUiRszIRS0QpMzQKMjKAQEjTAy5cgzSrSa1QLufSRZy7Z2l8wRGfmwTGOcSZqrkbgo_yXioqE0Abdng0Ka3iPWqdbSsgBvqG9m-3537AdVg6ND6NdF4ERoj9u2_DbVMvAtGc?purpose=inline)

**2. Operating Systems: Three Easy Pieces**

OS Concepts + Processes + Memory + Concurrency.

المرحلة 2

[The Linux Programming Interface by Michael Kerrisk System Programming Book                              –         Bookbeen](https://images.openai.com/static-rsc-4/PIiA8yrm992VqzNvmLaJKoob9F_i61qZTVglP3zSDR5Zvisuudu_GZyR6jzmIZAWSjivK3xYSJIvOMluAh325Q8tp2WmTCyBSnrwS5XXu1XRAVl7UKMPAUewca9Km7RcFUZxZ8xmm5cJxxzBr8lGD5lk2MCqr0hgjVHp7obk7ZE?purpose=inline)

**3. The Linux Programming Interface**

Linux System Calls + System Programming.

المرحلة 2–3

[‎Systems Performance by Brendan Gregg on Apple Books](https://images.openai.com/static-rsc-4/hsA1wFblRp8e2O8d_BYx2ixVES_NolCJjSdKpdC1jFtgX2hqcYXEsPKXBmwetV2wXUSj5NpiIcfHXeHQkoWhAydjnupVXt755mSGWjw4TS1_QT9OMuEYrmMdg2XlIAdlTpattuwOwAm-NZyjFdl85H8FCtEgqQ3gsbsLW83lIP4?purpose=inline)

**4. Systems Performance**

Performance Analysis + Optimization.

المرحلة 3

[C++ Concurrency in Action, Second Edition - Anthony Williams](https://images.openai.com/static-rsc-4/zUq2F9YCc3Qct3ifJiiwQL2DzSDnbhV-0AsR68A6Z8yM-NI_-_ys43wFn4Gi30kIc7p8PECNrxzeXdw6pfnDH__FL5isaF0zCqnxA0llPdPTd1Q2Khf_Z9_thxOuHON3cELuELkCciQbqbCa67vVCbXzd9k-sDGkcoT_JeJWiSg?purpose=inline)

**5. C++ Concurrency in Action**

Advanced C++ Concurrency.

المرحلة 4

[Programming Massively Parallel Processors (4th ed.)](https://images.openai.com/static-rsc-4/R-skP3fnM5LPfEqI9sx_6_4OwTi8aFDLk3ABr9Y1s9FH8ygqNaoUqI-I1hBuyNnM0FILgYXeseGvg5vw-bux8kpknSWFC7ctv2_o4d6q-aYiyn3ixRzFlp1541i_r66RI3Y-kmfH7FwkFhZRpjOgwVsSudoOvDVXIN05lYu9tUQ?purpose=inline)

**6. Programming Massively Parallel Processors**

GPU Programming + Parallel Computing.

المرحلة 5

أما في الجزء الأخير، فالمراجع الرئيسية ستكون وثائق CUDA وPyTorch وvLLM، وأبحاث Attention وFlashAttention، وكود المشاريع مفتوحة المصدر.

# **ثامناً: كيف نربط هذا كله في جدول زمني؟**

التقدير على أساس 10–12 ساعة أسبوعياً، وليس مواعيد إلزامية.

تقدير مدة كل مرحلة بالأسابيع، وفق المنهج المقترح.

0 أسبوع5 أسبوع10 أسبوع15 أسبوع20 أسبوعC FoundationComputer SystemsOS & LinuxAdvanced SystemsC++ SystemsCUDAInference FundamentalsInference EngineOptimization

# **96 أسبوعاً تقريباً**

24 شهراً وفق الجدول الكامل، مع هامش للمراجعة وإعادة المشاريع والتعمق.

**ملاحظة:** لا تنتقل آلياً بعد انتهاء الأسابيع. إذا لم تحقق مخرجات المرحلة، مددها. وقد تتداخل بعض المشاريع مع المراحل المجاورة.

# **تاسعاً: كيف تتعامل مع التعلم يومياً؟**

أقترح نظاماً ثابتاً لكل موضوع:

1. **افهم المفهوم**

   اقرأ من الكتاب، واكتب إجابة عن سؤال: لماذا توجد هذه التقنية؟ وما المشكلة التي تحلها؟
2. **شاهد التنفيذ**

   اقرأ Documentation أو مثالاً حقيقياً، وافحص الكود.
3. **نفذ تجربة صغيرة**

   لا تنتقل مباشرة إلى مشروع ضخم. جرب المفهوم منفرداً.
4. **استخدم Debugging**

   راقب الذاكرة والعمليات والـ System Calls أو GPU حسب المرحلة.
5. **أضف المفهوم إلى مشروع**

   إذا كان مناسباً، أضفه إلى مشروعك المتدرج.
6. **اكتب تقريراً هندسياً**

   ماذا تعلمت؟ ما الذي فشل؟ ما سبب الاختناق؟ ولماذا اخترت هذا التصميم؟

هذه الطريقة أفضل من مشاهدة 100 ساعة فيديو دون أن تستطيع بناء نظام بنفسك.

# **عاشراً: ما أول شيء تبدأ به الآن؟**

لا أنصحك أن تبدأ بشراء الكتب الستة أو تثبيت أدوات كثيرة.

ابدأ بثلاثة أشياء فقط:

**قائمة البداية**

First 30 Days

إنجاز المهام

## **0/6**

تجهيز بيئة C/C++ مع CMake وGDB وSanitizers

إنهاء مراجعة Pointers وMemory Management في C

فهم Compilation وLinking وObject Files

دراسة أول فصلين من CS:APP

بناء C Development Toolkit صغير

تجربة Debugging لبرنامج يعاني من Memory Leak

## **رأيي النهائي في اختيارك للتخصص**

أريد أن أضع نقطة مهمة أمامك:

أنت لديك خلفية في AI وDeep Learning وPython، لكن التخصص الذي اخترته سيأخذك إلى منطقة مختلفة عن بناء تطبيقات الذكاء الاصطناعي المعتادة.

بدلاً من أن يكون عملك مقتصراً على استخدام نموذج جاهز وبناء API حوله، ستتعلم كيف تُبنى الأنظمة التي تنفذ النموذج وتدير الذاكرة والطلبات والموارد.

وهناك ثلاثة مستويات مهنية يمكنك استهدافها مع تقدمك:

1. **Systems Software Engineer:** بناء برامج ومكتبات منخفضة المستوى.
2. **Inference Engineer:** تطوير وتحسين محركات تشغيل النماذج.
3. **AI Systems Engineer:** الجمع بين الأنظمة منخفضة المستوى والبنية التحتية للذكاء الاصطناعي.

المستوى الثالث هو الاتجاه الذي يمكن أن تبني نحوه تخصصك على المدى الطويل، دون أن تتسرع في ادعاء إتقانه قبل امتلاك الخبرة العملية.

مراجع رئيسية اعتمدنا عليها في تصميم المنهج:

- [CMU — Computer Systems: A Programmer's Perspective](https://csapp.cs.cmu.edu/3e/?utm_source=chatgpt.com).
- [OSTEP — Operating Systems](https://pages.cs.wisc.edu/~remzi/OSTEP/?utm_source=chatgpt.com).
- [The Linux Programming Interface](https://man7.org/tlpi/?utm_source=chatgpt.com).
- [NVIDIA CUDA Programming Guide](https://docs.nvidia.com/cuda/cuda-programming-guide/?utm_source=chatgpt.com).
- [vLLM Architecture](https://docs.vllm.ai/en/stable/design/arch_overview/?utm_source=chatgpt.com).

**وأخيراً، نصيحتي الأهم:** لا تتعامل مع هذا المنهج باعتباره 24 شهراً من الدراسة النظرية. اعتبره 24 شهراً من بناء مهارات هندسية ومشاريع متراكمة. مشروع Shell الذي بدأت به يمكن أن يكون أول لبنة في هذا المسار، ثم تتطور مشاريعك تدريجياً حتى تصل إلى بناء Inference Engine.&#x20;
