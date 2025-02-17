# 2025 Hagenberg meeting

\&nbsp;  
This week was the C++ Committee meeting, in Hagenberg, Austria 🇦🇹, on which we just finalized the C++26 feature freeze\!  
The features voted on will be added gradually to the working draft, and will likely be officially released on the next C++ version (C++26), barring any subsequent changes. This was the last meeting for forwarding C++26 features.  
The meeting site was the upper austria university of applied science, allowing the students to join the discussions as guests for the discussions. There was also an evening lecture (by organizers, with the participation of Herb, Bjarne and Jens) on which they could learn about the latest status of C++ and future directions\! 🧑‍🎓   
The hotel was convenient, and the meeting organizers ran the meeting wonderfully, with a lot of attention to details, including providing the menu schedule 🙂 (Thank you\!) The hybrid (on-site/online) experience worked as expected. We appreciate that greatly\!   
We will continue operating hybrid meetings going forward.  
\&nbsp;  
Main C++26 Features approved in Hagenberg: 🎉

\* \[P2900R14\](https://wg21.link/P2900): Contracts for C++  
\* \[P2786R13\](https://wg21.link/P2786): Trivial Relocatability For C++26  
\* \[P2841R7\](https://wg21.link/P2841): Concept and variable-template template-parameters  
\* \[P3471R3\](https://wg21.link/P3471R3): Standard Library Hardening  
\* \[P0260R15\](https://wg21.link/P0260R15): C++ Concurrent Queues  
\* \[P3179R6\](https://wg21.link/P3179R6): C++ parallel range algorithms  
\* \[P3070R2\](https://wg21.link/P3070R2): Formatting \~\~enums\~\~ (was \`enums\` only, extended to user defined types)

We also rebased C++26 on C23 by approving: “\[P3348R1\](https://wg21.link/P3348R1): C++26 should refer to C23 not C17” (thank you, Jonathan Wakely\!)

We had 201 attendees attending the Hagenberg meeting: 128 were in person, and 73 were virtual.

\&nbsp;

\*\*\*\*\*

\# Language Progress

\*\*\*\*\*

\&nbsp;

\*\*\*\*\*

\#\#\# Evolution Working Group (EWG) Progress

\*\*\*\*\*

\&nbsp;

This week, EWG saw 56 papers and resolved 7 issues. The objective was to finalize C++26 features, "all bugs in". Meetings going forward will have EWG fixing any bugs for C++26, and reviewing features for C++29.    
\&nbsp;

\*\*おつかれさまです！🙏\*\*  
\&nbsp;

\#\#\# 📝 Contracts

⏩ contracts are in C++26, polls \[on the P2900 tracker\](https://github.com/cplusplus/papers/issues/1648\#issuecomment-2651224887)  

\&nbsp;

This week we:

\* reviewed significant feedback    
\* disallowed pre/post contracts on virtual functions entirely    
\* contended, but unchanged: exceptions when they leave predicate evaluation

\&nbsp;

📈 Consensus on contracts has increased since the last meeting. 📈    
Thank you to all the authors, and everyone who's provided feedback\\\! Contracts in C++26 are a huge deal for programmers who want to increase their code's correctness and quality.  

\&nbsp;

Papers considered:

\* ❌ \[P3573\](https://wg21.link/p3573r0) — \[Contract concerns\](https://github.com/cplusplus/papers/issues/2215)    
\* ❌ \[P3506\](https://wg21.link/p3506r0) — \[P2900 Is Still not Ready for C++26\](https://github.com/cplusplus/papers/issues/2192)    
\* ❌ \[P3591\](https://wg21.link/P3591r0) — \[Contextualizing Concerns About Contracts\](https://github.com/cplusplus/papers/issues/xxx)    
\* ❌ \[P3500\](https://wg21.link/p3500r0) — \[Are Contracts "safe"?\](https://github.com/cplusplus/papers/issues/2190)    
\* ❌ \[P3577\](https://wg21.link/P3577r0) — \[Require a non-throwing default contract-violation handler\](https://github.com/cplusplus/papers/issues/2219)    
\* ❌ \[P3229\](https://wg21.link/p3229r0) — \[Making erroneous behaviour compatible with Contracts\](https://github.com/cplusplus/papers/issues/2186)    
\* ❌ \[P3269\](https://wg21.link/p3269r0) — \[Do Not Ship Contracts as a TS\](https://github.com/cplusplus/papers/issues/1925)    
\* ❌ \[P3265\](https://wg21.link/p3265r3) — \[Ship Contracts in a TS\](https://github.com/cplusplus/papers/issues/1921)

\#\#\# 📋 Profiles

We reviewed the following papers on profiles:

\* ✅ \[P3589\](https://wg21.link/p3589r0) — \[C++ Profiles: The Framework\](https://github.com/cplusplus/papers/issues/2232)    
\* ✅ \[P3611\](https://wg21.link/P3611R0) — \[Dealing with pointer errors: Separating static and dynamic checking\](https://github.com/cplusplus/papers/issues/xxx)    
\* ✅ \[P3081\](https://wg21.link/p3081r1) — \[Core safety profiles for C++26\](https://github.com/cplusplus/papers/issues/2058)    
\* ❌ \[P3586\](https://wg21.link/p3586r0) — \[The Plethora of Problems With Profiles\](https://github.com/cplusplus/papers/issues/2229)    
\* ❌ \[P3543\](https://wg21.link/p3543r0) — \[Response to Core Safety Profiles (P3081)\](https://github.com/cplusplus/papers/issues/2180)    
\* ✅ \[P3447\](https://wg21.link/p3447r0) — \[Profiles syntax\](https://github.com/cplusplus/papers/issues/2111)    
\* ❌ \[P3599\](https://wg21.link/P3599r0) — \[Initial Implicit Contract Assertions\](https://github.com/cplusplus/papers/issues/xxx)    
\* ✅ \[P3274\](https://wg21.link/p3274r0) — \[A framework for Profiles development\](https://github.com/cplusplus/papers/issues/1929)    
\* ❌ \[P3541\](https://wg21.link/p3541r1) — \[Violation handlers vs \\\`noexcept\\\`\](https://github.com/cplusplus/papers/issues/2178)

\&nbsp;  
\#\#\#\# For profiles, we voted the following:  

Pursue a language safety white paper in the C++26 timeframe containing systematic treatment of core language Undefined Behavior in C++, covering Erroneous Behavior, Profiles, and Contracts. Appoint Herb and Gašper as editors.  

\&nbsp;  
\&nbsp;

What does this mean?    
\&nbsp;  
Many people felt that what profiles are trying to address (security, safety) is hugely critical... yet profiles as they stand today are not ready. The C++26 train is leaving the station, but we want progress, now\!    
\&nbsp;

\#\#\#\# \<white\_paper\> 

What are White Papers?

White papers are a tool that ISO is now encouraging us to use, whereby we need WG21 plenary approval and SC22 approval, and then we have an approved white paper. The implication: We can get profiles in a white paper, implemented in compilers (behind a flag) before C++26 is finalized.    
\&nbsp;  
How does that work? White papers are a lightweight TS, or a heavy paper. The way we manage this is fairly open and we heard concerns which Herb and Gašper will suggest ways to address. For now, we have them as editors, they choose what goes in the white paper, and our hope is that they are trusted by everyone to do so while increasing consensus. EWG will see updates, forward them to CWG, then to plenary, then SC22, with votes at each stop. This is actually lightweight, and will allow rapid improvements and feedback. One way to address issues brought up is to have a git repo on github.com/cplusplus where the white paper is developed, with great commit messages, with periodic reports (say, monthly), and with periodic EWG telecons to review (say, monthly). Herb and Gašper will publish details soon.    
\&nbsp;  
Of course, we cannot take implementations for granted. A white paper is a new tool, but we can't be shipping unstable white papers every week and expect implementations to ship them. But we know white papers will be lower overhead than a TS. We therefore expect that white paper editors will be mindful editors.    
\&nbsp;  
What is expected in the white paper? systematic treatment of core language Undefined Behavior in C++, covering Erroneous Behavior, Profiles, and Contracts. This is broad\\\! The final white paper doesn't need to include all of these, but it's the scope that was given to them. The idea is to try to comprehensively address security and safety issues, and do so with a comprehensive design. The scope given to the white paper allows aligning these topics, together. Contracts are in C++26, but profiles will likely be usable in a production compiler before contracts are usable behind \\-std=c++26. This is great for contracts as well\\\! It means that we'll be able to address perceived shortcomings of contracts with respect to safety rapidly, with direct feedback, in the C++29 timeframe thanks to the white paper.  

\#\#\#\# \</white\_paper\>

\&nbsp;

Why Herb and Gašper? Throughout the years they've shown themselves to be mediators, and great at obtaining consensus from groups who have a hard time agreeing. Herb is indefatigable, and has in the last few months put in incredible efforts in advancing a variety of proposals. Gašper goes into details and synthesizes it into consensus, we've seen this in action in contracts to help bridge gaps that seemed unbridgeable. The thinking is that they complement each other, and are well trusted by a variety of committee members to fairly take feedback and advance this critical topic.    
\&nbsp;  
This is a huge undertaking for both of them. Herb has signed up to dedicate 1.5 to 2 years of his life almost full-time on improving C++ safety and security. Thank you Herb\\\! While Gašper wasn't here for this meeting, he's also signed up for significant work. Thank you\\\!

\#\#\# 🍱 Various C++26 papers

\* ✅ \[P2841\](https://wg21.link/p2841r7) — \[Concept and variable-template template-parameters\](https://github.com/cplusplus/papers/issues/1546)    
\* ✅ \[P2786\](https://wg21.link/p2786r11) — \[Trivial Relocatability For C++26\](https://github.com/cplusplus/papers/issues/1463)    
\* ✅ \[P3310\](https://wg21.link/p3310r5) — \[Solving issues introduced by relaxed template template parameter matching\](https://github.com/cplusplus/papers/issues/1961)    
\* ✅ \[P2719\](https://wg21.link/p2719r2) — \[Type-aware allocation and deallocation functions\](https://github.com/cplusplus/papers/issues/1898)    
\* ✅ \[P2866\](https://wg21.link/p2866r5) — \[Remove Deprecated Volatile Features From C++26\](https://github.com/cplusplus/papers/issues/1556)    
\* ✅ \[P2843\](https://wg21.link/p2843r1) — \[Preprocessing is never undefined\](https://github.com/cplusplus/papers/issues/1548)    
\* ✅ \[P2287\](https://wg21.link/p2287r3) — \[Designated-initializers for base classes\](https://github.com/cplusplus/papers/issues/978)    
\* ✅ \[P3501\](https://wg21.link/P3501r0) — \[The ad-dressing of cats\](https://github.com/cplusplus/papers/issues/2191) (note: no cats were present)    
\* ✅ \[P0149\](https://wg21.link/D0149r2) — \[Generalised member pointers\](https://github.com/cplusplus/papers/issues/2223)    
\* ✅ \[P3618\](https://wg21.link/P3618r0) — \[Allow attaching main to the global module\](https://github.com/cplusplus/papers/issues/2237)    
\* ✅ \[P2825\](https://wg21.link/p2825r4) — \[Overload resolution hook: declcall( unevaluated-call-expression )\](https://github.com/cplusplus/papers/issues/1503)    
\* ✅ \[P3492\](https://wg21.link/p3492r0) — \[Sized deallocation for placement new\](https://github.com/cplusplus/papers/issues/2144)    
\* ✅ \[P2952\](https://wg21.link/p2952r2) — \[auto& operator=(X&&) \\= default\](https://github.com/cplusplus/papers/issues/1624)    
\* ✅ \[P1967\](https://wg21.link/p1967r14) — \[\\\#embed \\- a simple, scannable preprocessor-based resource acquisition method\](https://github.com/cplusplus/papers/issues/700)    
\* ✅ \[P3540\](https://wg21.link/P3540r0) — \[\\\`\\\#embed\\\` offset parameter\](https://github.com/cplusplus/papers/issues/2238)    
\* ✅ \[P1306\](https://wg21.link/p1306r3) — \[Expansion statements\](https://github.com/cplusplus/papers/issues/156)    
\* ✅ \[P3074\](https://wg21.link/p3074r5) — \[trivial unions (was std::uninitialized)\](https://github.com/cplusplus/papers/issues/1734)    
\* ✅ \[P3471\](https://wg21.link/P3471r3) — \[Standard Library Hardening: forward to CWG for inclusion in C++26\](https://github.com/cplusplus/papers/issues/2125) this is a huge deal for safety and security    
\* ✅ \[P3111\](https://wg21.link/p3111r3) — \[Atomic Reduction Operations\](https://github.com/cplusplus/papers/issues/1902)    
\* ✅ Transactional Memory TS to a white paper    
\* ♻️ \[P3006\](https://wg21.link/P3006r2) — \[Launder less\](https://github.com/cplusplus/papers/issues/1703)    
\* ♻️ \[P0876\](https://wg21.link/p0876r19) — \[fiber\\\_context \\- fibers without scheduler\](https://github.com/cplusplus/papers/issues/117)    
\* 🌊 \[P3568\](https://wg21.link/P3568r0) — \[break label; and continue label;\](https://github.com/cplusplus/papers/issues/2212) (only input for WG14, with not strong preference either direction, but interested in this feature)    
\* ⚠️ \[P2434\](https://wg21.link/p2434r3) — \[Nondeterministic pointer provenance\](https://github.com/cplusplus/papers/issues/1364) (prospective pointer value was taken out, otherwise back in CWG)    
\* ❌ \[P2883\](https://wg21.link/p2883r1) — \[\\\`offsetof\\\` Should Be A Keyword In C++26\](https://github.com/cplusplus/papers/issues/1560)    
\* ❌ \[P3477\](https://wg21.link/p3477r2) — \[There are exactly 8 bits in a byte\](https://github.com/cplusplus/papers/issues/2131)    
\* ❌ \[P3232\](https://wg21.link/p3232r1) — \[User-defined erroneous behaviour\](https://github.com/cplusplus/papers/issues/1877)    
\* ❌ \[P3439\](https://wg21.link/p3439r1) — \[Chained comparisons: Safe, correct, efficient\](https://github.com/cplusplus/papers/issues/2103)

\&nbsp;  
Paper P2843 "Preprocessing is never undefined" above resolves the following issues:

\* ✅ \[CWG2577\](https://wg21.link/CWG2577) — \[Undefined behavior for preprocessing directives in macro arguments\](https://github.com/cplusplus/papers/issues/1413)    
\* ✅ \[CWG2581\](https://wg21.link/CWG2581) — \[Undefined behavior for predefined macros\](https://github.com/cplusplus/papers/issues/1412)    
\* ✅ \[CWG2580\](https://wg21.link/CWG2580) — \[Undefined behavior with \\\#line\](https://github.com/cplusplus/papers/issues/1411)    
\* ✅ \[CWG2579\](https://wg21.link/CWG2579) — \[Undefined behavior when token pasting does not create a preprocessing token\](https://github.com/cplusplus/papers/issues/1410)    
\* ✅ \[CWG2578\](https://wg21.link/CWG2578) — \[Undefined behavior when creating an invalid string literal via stringizing\](https://github.com/cplusplus/papers/issues/1409)    
\* ✅ \[CWG2576\](https://wg21.link/CWG2576) — \[Undefined behavior with macro-expanded \\\#include directives\](https://github.com/cplusplus/papers/issues/1408)    
\* ✅ \[CWG2575\](https://wg21.link/CWG2575) — \[Undefined behavior when macro-replacing "defined" operator\](https://github.com/cplusplus/papers/issues/1407)

\#\#\# 🪞 Reflection

\&nbsp;  
Reflection: "the renaissance of C++"    
\&nbsp;  
Reflection is still in C++26\\\! This week we:

\* added access control, need to opt-in to unchecked    
\* add function parameter reflection    
\* add immediate-escalating expressions

\&nbsp;  
Papers seen:

\* ❌ \[P3587\](https://wg21.link/p3587r0) — \[Reconsider reflection access for C++26\](https://github.com/cplusplus/papers/issues/2230)    
\* ✅ \[P3547\](https://wg21.link/p3547r0) — \[Modeling Access Control With Reflection\](https://github.com/cplusplus/papers/issues/2196)    
\* ✅ \[P3096\](https://wg21.link/p3096r5) — \[Function Parameter Reflection in Reflection for C++26\](https://github.com/cplusplus/papers/issues/1764)    
\* ✅ \[P3496\](https://wg21.link/p3496r0) — \[Immediate-Escalating Expressions\](https://github.com/cplusplus/papers/issues/2189)    
\* ❌ \[P3569\](https://wg21.link/p3569r0) — \[Split define\\\_aggregate from Reflection\](https://github.com/cplusplus/papers/issues/2213)    
\* ✅ \[D2996R10\](https://wiki.edg.com/pub/Wg21hagenberg2025/EvolutionWorkingGroup/d2996r10.html\#design-changes-since-p2996r4) — \[Reflection for C++26\](https://github.com/cplusplus/papers/issues/1668) (changes back from CWG which needs our approval)

\#\#\# 🧊 \`constexpr\`

\* ✅ \[P3533\](https://wg21.link/P3533r1) — \[constexpr virtual inheritance\](https://github.com/cplusplus/papers/issues/2174)    
\* ✅ \[P3590\](https://wg21.link/p3590r0) — \[Constexpr Coroutines Burdens\](https://github.com/cplusplus/papers/issues/2233)    
\* ✅ \[P3367\](https://wg21.link/p3367r3) — \[constexpr coroutines\](https://github.com/cplusplus/papers/issues/2069) voted, but for C++29

\#\#\# 🐾 Pattern matching

Pattern matching: "We hardly knew ye"    
\&nbsp;  
Pattern matching did not get consensus, but it was extremely close. Attendees felt that it wasn't quite ready for C++26. Let’s get it in C++29\!    
\&nbsp;  
Main papers which were discussed:

\* ✅ \[P3572\](https://wg21.link/p3572r0) — \[Pattern matching\](https://github.com/cplusplus/papers/issues/2214)    
\* ✅ \[P2688\](https://wg21.link/p2688r5) — \[Pattern Matching: \\\`match\\\` Expression\](https://github.com/cplusplus/papers/issues/1353)

\&nbsp;  
Library parts, not discussed this meeting:

\* \[P3527\](https://wg21.link/p3527r1) — \[Pattern Matching: \*\*variant-like\*\* and \\\`std::expected\\\`\](https://github.com/cplusplus/papers/issues/2172)    
\* \[P3521\](https://wg21.link/p3521r0) — \[Pattern Matching: Customization Point for Open Sum Types\](https://github.com/cplusplus/papers/issues/2169)

\&nbsp;

\*\*\*\*\*

\#\#\# Evolution Working Group Incubator Study Group (SG17) Progress

\*\*\*\*\*

EWGI discussed 7 papers during the day on Wednesday.  Of these, 4 were forwarded to EWG, 3 were seen and will be seen again. 

\#\#\#\# Papers Forwarded to EWG

\* \[P3412R1\](https://wg21.link/P3412R1): String Interpolation — This paper proposes ‘f’ strings (and a similar ‘x’ string) that allows in-string expressions, which are handled at preprocessor time to expand to a call to std::format, or arguments compatible with std::format.  
\* \[P3424R0\](https://wg21.link/P3424R0): Define Delete with Throwing Exception Specification  — This paper attempts to remove a piece of undefined behavior by making a ‘noexcept(\<false-expr\>)’ production deprecated, which prevents undefined behavior.  
\* \[P2490R3\](https://wg21.link/P2490R3): Zero-overhead exception stack traces — An attempt to expose stack traces in catch handlers that opt-in.  
\* \[P3588R0\](https://wg21.link/P3588R0): Allow static data members in local and unnamed classes — This paper attempts to remove an old restriction on data members of local and unnamed classes.

\#\#\#\# Papers that got feedback and will be seen again by EWGI

\* \[P3550R0\](https://wg21.link/P3550R0): Imports cannot… — A modules based paper that attempts to make C variadic functions ill-formed outside of the global namespace. The author received feedback that this is likely not acceptable due to type-trait-like classes.  
\* \[P3530R0\](https://wg21.link/P3530R0): Intrinsic for reading uninitialized memory — This paper explores and proposes 2 alternatives for managing uninitialized memory, and reading it in a non-undefined behavior method.  
\* \[P3568R0\](https://wg21.link/P3568R0): break label; and continue label; — This paper proposes to expose the C feature of a similar name to C++.  However, this feature is contentious/has alternatives being considered, so the author requested feedback on what he could tell the WG14 committee is our preference.

\&nbsp;

\*\*\*\*\*

\#\#\# Core Working Group (CWG) Progress

\*\*\*\*\*

CWG met during the full week, and reviewed papers targeting C++26, including reflection. We approved the wording for contracts, which were voted in C++26.  
We also approved resolutions for \[CWG2549\](https://wg21.link/CWG2549),  \[CWG2703\](https://wg21.link/CWG2703), \[CWG2943\](https://wg21.link/CWG2943),   
\[CWG2970\](https://wg21.link/CWG2970), and \[CWG2990\](https://wg21.link/CWG2990).

As the next meeting (Sofia) is the last meeting for C++26 papers, our primary focus  
is on reviewing the wording of papers approved by EWG for C++26. most notably reflection. We will hold telecons to make progress ahead of the next meeting. 

\#\#\#\# Papers reviewed and sent to plenary (apply changes to the C++ Working Paper)

\* \[P3542R0\](https://wg21.link/P3542R0): Abolish the term "converting constructor"  
\* \[P3074R7\](https://wg21.link/P3074): trivial unions (was std::uninitialized)  
\* \[P1494R5\](https://wg21.link/P1494): Partial program correctness  
\* \[P2900R14\](https://wg21.link/P2900): Contracts for C++  
\* \[P3475R2\](https://wg21.link/P3475): Defang and deprecate memory\_order::consume  
\* \[P2841R7\](https://wg21.link/P2841): Concept and variable-template template-parameters  
\* \[P2786R13\](https://wg21.link/P2786): Trivial Relocatability For C++26  
\* \[P1967R14\](https://wg21.link/P1967): \#embed \- a simple, scannable preprocessor-based resource acquisition method

\#\#\#\# Papers which will need to be seen again by CWG

\* \[P2843R1\](https://wg21.link/P2843R1): Preprocessing is never undefined. This paper removes UB from the preprocessor by making some constructs either ill-formed, or well-defined. We gave some feedback to the author and expect to approve it at a future meeting. This continues to remove UB outside of evaluation.

\* \[P2719R3\](https://wg21.link/P2719R3): Type-aware allocation and deallocation functions. This paper proposes a new \`new\` overload taking a type\_identity. This can be used to have per-type allocation buckets, which reduces type confusion vulnerabilities. We gave feedback on the wording to the author and expect to see this again. This paper is currently targeting C++26

\* \[P3421R0\](https://wg21.link/P3421R0): Consteval destructors

\* \[P2996\](https://wg21.link/P2996): Reflection

\&nbsp;

\*\*\*\*\*

\# Library Progress

\*\*\*\*\*  
\&nbsp;

\*\*\*\*\*

\#\#\# Library Evolution Working Group (LEWG) Progress

\*\*\*\*\*

\&nbsp;

LEWG met during the full week, and reviewed 45 papers. We’ve been working mostly on improvements and fixes to our main features targeting C++26, but we also had a chance to have some smaller neat additions\! 

\#\#\#\# Main Topics Discussed  
(for topics already forwarded, we discussed improvements / fixes)  
\* Sender Receiver (\[P2300\](https://wg21.link/P2300) (forwarded in \[St. Louis\](https://www.reddit.com/r/cpp/comments/1dwc7f2/202406\_st\_louis\_iso\_c\_committee\_trip\_report/)))  
\- Reflection (\[P2996\](https://wg21.link/P2996) (targeting Sofia))  
\- SIMD (\[P1928\](https://wg21.link/P1928) (forwarded in \[wrocław\](https://www.reddit.com/r/cpp/comments/1ienpc7/202411\_wroc%C5%82aw\_iso\_c\_committee\_trip\_report\_fifth/)   
\- Trivial Relocatability (\[P2786\](https://wg21.link/P2786) (forwarded in \[Tokyo\](https://www.reddit.com/r/cpp/comments/1bloatw/202403\_tokyo\_iso\_c\_committee\_trip\_report\_third/))  
\- Concurrent Qs (\[P0260\](https://wg21.link/P0260) (forwarded during this meeting))  
\- Standard Library Hardening (\[P3471\](https://wg21.link/P3471) forwarded during this meeting)  
\- Ranges (\[P0896\](https://wg21.link/P0896), \[P2214R1\](https://wg21.link/P2214R1), \[P2214R2\](https://wg21.link/P2214R2) (accepted for C++20, additions since)  
\&nbsp;  
\- \[P3348R1\](https://wg21.link/P3348R1): C++26 should refer to C23 not C17 — rebasing C++ on C\! (thank you, Jonathan Wakely\!)

\&nbsp;

\#\#\#\# Papers forwarded to LWG

\#\#\#\#\# Reflection

\* ✅ \[P3394R1\](https://wg21.link/P3394R1): Annotations for Reflection — new feature allowing users to append information for reflection to build upon  
\* ✅ \[P3293R1\](https://wg21.link/P3293R1): Splicing a base class subobject — addresses concerns  
\* ✅ \[P3491R1\](https://wg21.link/P3491R1): define\_static\_(string,object,array) — adds compile time structures improving usability of reflection   
\* ✅ \[P3547R1\](https://wg21.link/P3547R1): Modeling Access Control With Reflection — address concerns raised regarding access  
\* ✅ \[P3560R0\](https://wg21.link/P3560R0): Error Handling in Reflection — adds \`std::meta::exception\`, utilize constexpr exceptions to improve error reporting in reflection

\#\#\#\# Senders Receivers

\* ✅ \[P2079R7\](https://wg21.link/P2079R7): Parallel Scheduler (was: System Execution Context) — addition for managing execution context  
\* ✅ \[P3149R8\](https://wg21.link/P3149R8): async\_scope \-- Creating scopes for non-sequential concurrency — addition for managing async-sync integration  
\* ✅ \[P3296R3\](https://wg21.link/P3296R3): let\_async\_scope — managing async-sync integration, designed to provide simpler default  
\* ✅ \[P3481R2\](https://wg21.link/P3481R2): std::execution::bulk() issues — improvements to utility (joined paper with “\[P3564R0\](https://wg21.link/P3564R0) Make the concurrent forward progress guarantee usable in \`bulk\`” thank you to the authors for working together to merge the papers\!)  
\* ✅ \[P3570R0\](https://wg21.link/P3570R0): Optional variants in sender/receiver — utility for improved integration with coroutines   
\* ✅ \[P3164R3\](https://wg21.link/P3164R3): Early Diagnostics for Sender Expressions — improved errors\!  
\* ✅ \[P3557R0\](https://wg21.link/P3557R0): High-Quality Sender Diagnostics with Constexpr Exceptions — utilize constexpr exceptions for senders\!  
\* ✅ \[P3425R2\](https://wg21.link/P3425R2): Reducing operation-state sizes for sub-object child operations — optimization  
\* ✅ \[P3433R0\](https://wg21.link/P3433R0): Allocator Support for Operation States — improvement

\#\#\#\# Safety  
\* ✅ \[P3471R3\](https://wg21.link/P3471R3): Standard Library Hardening — turning preconditions into hardened ones, provides stronger guarantees.

\#\#\#\# Other Features

\* ✅ \[P3516R0\](https://wg21.link/P3516R0): Uninitialized algorithms for relocation — library interface for Relocatability  
\* ✅ \[P2988R9\](https://wg21.link/P2988R9): std::optional\<T&\> — adding support for ref types in optional  
\* ✅ \[P0260R15\](https://wg21.link/P0260R15): C++ Concurrent Queues — concurrent container\!  
\* ✅ \[P3179R6\](https://wg21.link/P3179R6): C++ parallel range algorithms  
\* ✅ \[P3070R2\](https://wg21.link/P3070R2): Formatting \~\~enums\~\~ (was \`enums\` only, extended to all user defined types) — easier way to define formatters for users  
\* ✅ \[P3111R3\](https://wg21.link/P3111R3): Atomic Reduction Operations — API extension  
\* ✅ \[P3383R1\](https://wg21.link/P3383R1): mdspan.at() — API addition  
\* ✅ \[P3044R0\](https://wg21.link/P3044R0): sub-string\_view from string — API addition   
\* ✅ \[P3060R2\](https://wg21.link/P3060R2): Add std::views::indices(n) — avoid off by one  
\* ✅ \[P1317R1\](https://wg21.link/P1317R1): Remove return type deduction in std::apply — fixes  
\* ✅ \[P3623R0\](https://wg21.link/P3623R0): Add noexcept to \[iterator.range\] (LWG 3537\) —   
\* ✅ \[P3567R0\](https://wg21.link/P3567R0): \`flat\_meow\` Fixes — fixes  
\* ✅ \[P3016R5\](https://wg21.link/P3016R5): Resolve inconsistencies in begin/end for valarray and braced initializer lists — fixes  
\* ✅ \[P3037R4\](https://wg21.link/P3037R4): constexpr std::shared\_ptr — extension  
\* ✅ \[P3416R2\](https://wg21.link/P3416R2): exception\_ptr\_cast: Add && \= delete overload — fixes  
\* ✅ \[P2319R4\](https://wg21.link/P2319R4): Prevent path presentation problems — API update (Breaking Change, fixes \`filesystem::path\`) 

\&nbsp;

\#\#\#\# Papers / issues sent from LWG seen by LEWG

\* ✅ \[P3019R13\](https://wg21.link/P3019R13): Vocabulary Types for Composite Class Design — apply design changes, send back to LWG  
\* ✅ \[P2019R7\](https://wg21.link/P2019R7): Thread Attributes — apply SG16 recommendation, send back to LWG  
\* ✅ \[P2663R6\](https://wg21.link/P2663R6): Proposal to support interleaved complex values in std::simd — approved, sent back to LWG  
\* ✅ \[P2664R9\](https://wg21.link/P2664R9): Proposal to extend std::simd with permutation API — approved, sent back to LWG  
\* ✅ \[P2993R3\](https://wg21.link/P2993R3): Extend \<bit\> header function with overloads for std::simd — approved, sent back to LWG  
\&nbsp;

\#\#\#\# Papers that got feedback and will be seen again by LEWG

\* 🔄 \[P3552R0\](https://wg21.link/P3552R0): Add a Coroutine Lazy Type  
\* 🔄 \[P3380R1\](https://wg21.link/P3380R1): Extending support for class types as non-type template parameters — no implementation, requires more work (reflection)

\&nbsp;

\#\#\#\# Papers that did not get consensus

\* ❌ \[P3559R0\](https://wg21.link/P3559R0): Trivial relocation: One trait or two?  
\* ❌ \[P3477R1\](https://wg21.link/P3477R1): There are exactly 8 bits in a byte  
\* ❌ \[P3160R2\](https://wg21.link/P3160R2): An allocator-aware \`inplace\_vector\`

\#\#\#\# Policies discussion

We will resume our discussion about policies in Sofia\!

Information about policies can be found in: “\[[P2267](https://wg21.link/P2267)R1\](https://wg21.link/p2267r1): Library Evolution Policies (The rationale and process of setting a policy for the Standard Library)”.

We will discuss the following topics:

\* Explicit Constructors  
\* Overload resolution with concepts  
\* Unicode support (Collaboration with SG16)

Worth noting that Evolution Work Group (EWG) have also introduced policies, and have accepted: “\[SD-10\](https://isocpp.org/std/standing-documents/sd-10-language-evolution-principles): Language Evolution (EWG) Principles” during Wroclaw.

\&nbsp;

\#\#\#\# Evening Sessions

In addition to the work meeting, we had two evening sessions during the week (initiated by WG21 members).   
Evening sessions are informative sessions, during which we do not take any binding votes. 

They are meant for either reviewing topics relevant to the committee in more depth than possible during the work sessions (such is the case for "Relocatability") , or for introducing topics which are not procedurally related but are relevant to WG21 (such is the case for “Perspectives on Contracts").

\* 🔎Tuesday: “Concurrent Queues”

\&nbsp;

Thank you to all our authors and participants, for a great collaboration in a productive and useful review process, and see you (in-person or online) in Sofia\!◝(ᵔᵕᵔ)◜

\&nbsp;

\*\*\*\*\*

\#\#\# Library Evolution Working Group Incubator Study Group (SG18) Progress

LEWGI/SG18 did not meet in person during Hagenberg (to allow more time to focus on C++26 design freeze) but will be holding regular telecons, usually only looking at one paper and giving the author feedback so that their paper is in the best possible shape for consideration by LEWG or various other study groups.  SG18 planning on meeting in person in Sofia.

\&n debsp;

\*\*\*\*\*

\#\#\# Library Working Group (LWG) Progress

\*\*\*\*\*

LWG met in person throughout the week and reviewed multiple papers.

\&nbsp;

\#\#\#\# Papers forwarded to plenary  
\* \[P3137R3\](https://wg21.link/P3137R3): views::to\_input  
\* \[P0472R3\](https://wg21.link/P0472R3): Put std::monostate in ⟨utility⟩ — the C++ working paper  
\* \[P3349R1\](https://wg21.link/P3349R1): Converting contiguous iterators to pointers  
\* \[P3372R3\](https://wg21.link/P3372R3): constexpr containers and adaptors  
\* \[P3378R2\](https://wg21.link/P3378R2): constexpr exception types  
\* \[P3441R2\](https://wg21.link/P3441R2): Rename simd\_split to simd\_chunk  
\* \[P3287R3\](https://wg21.link/P3287R3): Exploration of namespaces for std::simd  
\* \[P2976R1\](https://wg21.link/P2976R1): Freestanding Library: algorithm, numeric, and random  
\* \[P3430R3\](https://wg21.link/P3430R3): simd issues: explicit, unsequenced, identity-element position, and members of disabled simd  
\* \[P2663R7\](https://wg21.link/P2663R7): Interleaved complex values support in std::simd  
\* \[P2933R4\](https://wg21.link/P2933R4): Extend ⟨bit⟩ header function with overloads for std::simd  
\* \[P2846R6\](https://wg21.link/P2846R6): reserve\_hint: Eagerly reserving memory for not-quite-sized lazy ranges  
\* \[P3471R4\](https://wg21.link/P3471R4): Standard Library Hardening  
\* \[P0447R28\](https://wg21.link/P0447R28): Introduction of std::hive  
\* \[P3019R14\](https://wg21.link/P3019R14): indirect and polymorphic: Vocabulary Types for Composite Class Design

\&nbsp;

\#\#\#\# Papers that require more LWG review time  
\* \[P3096R6\](https://wg21.link/P3096R6): Function Parameter Reflection in Reflection for C++26  
\* \[P2996R10\](https://wg21.link/P2996R10): Reflection for C++26  
\* \[P3284R2\](https://wg21.link/P3284R2): write\_env and unstoppable Sender Adaptors  
\* \[P3149R8\](https://wg21.link/P3149R8): async\_scope – Creating scopes for non-sequential concurrency	35  
\* \[P2781R6\](https://wg21.link/P2781R6): std::constant\_wrapper  
\* \[P3472R3\](https://wg21.link/P3472R3): Make fiber\_context::can\_resume() const	58  
\* \[D2988R10\](https://wg21.link/D2988R10): std::optional\<T&\>  
\* \[P3179R7\](https://wg21.link/P3179R7): C++ parallel range algorithms

\&nbsp;

\#\#\#\# Issues Reviewed by LWG  
\* \[LWG4198\](https://wg21.link/LWG4198): schedule\_from isn't starting the schedule sender if decay-copying results throws  
\* \[LWG4198\](https://wg21.link/LWG4198): schedule\_from isn't starting the schedule sender if decay-copying results throws	16  
\* \[LWG4199\](https://wg21.link/LWG4199): ​​constraints on user customizations of standard sender algorithms are incorrectly specified	16  
\* \[LWG4202\](https://wg21.link/LWG4202): enable-sender should be a variable template	17  
\* \[LWG4203\](https://wg21.link/LWG4203): Constraints on get-state functions are incorrect	17  
\* \[LWG4204\](https://wg21.link/LWG4204): specification of as-sndr2(Sig) in \[exec.let\] is incomplete	18  
\* \[LWG4205\](https://wg21.link/LWG4205): let\_\[\*\].transform\_env is specified in terms of the let\_\* sender itself instead of its child	18  
\* \[LWG4206\](https://wg21.link/LWG4206): Alias template connect\_result\_t should be constrained with sender\_to	18  
\* \[LWG4208\](https://wg21.link/LWG4208): Wording needs to ensure that in connect(sndr, rcvr) that rcvr expression is only evaluated once	19  
\* \[LWG4209\](https://wg21.link/LWG4209): default\_domain::transform\_env should be returning FWD-ENV(env)	19

\&nbsp;  
\#\#\#\# Papers forwarded to other groups (CWG/LEWG)  
\* \[P2830R9\](https://wg21.link/P2830R9): Standardized Constexpr Type Ordering) — finalized review, to be approved by CWG

Note: Issues finalized during a meeting are tentatively ready but voted on during the next meeting (in this case, Hagenberg).

\&nbsp;

\*\*\*\*\*

\# Study Group Progress

\*\*\*\*\*  
\&nbsp;

\*\*\*\*\*

\#\#\# Concurrency and Parallelism Study Group (SG1) Progress

\*\*\*\*\*

\#\#\#\# Papers forwarded to LEWG/EWG

\* \[P2079R6\](https://wg21.link/P2079R6): System execution context \- forwarded to LEWG  
\* \[P3501R0\](https://wg21.link/P3501R0): The ad-dressing of cats \- forwarded to EWG  
\* \[P3481R1\](https://wg21.link/P3481R1): std::execution::bulk() issues \- forwarded to LEWG  
\* \[P3552R0\](https://wg21.link/P3552R0): Add a Coroutine Lazy Type \- forwarded to LEWG  
\* \[P3366R0\](https://wg21.link/P3366R0): Remove Deprecated Atomic Initialization API from C++26 \- forwarded to LEWG  
\* \[P0260R14\](https://wg21.link/P0260R14): Concurrent Queue \- forwarded to LEWG  
\* \[P3347R1\](https://wg21.link/P3347R1): Invalid/Prospective Pointer Operations \- forwarded to EWG  
\* \[P2414R6\](https://wg21.link/P2414R6): Pointer lifetime-end zap proposed solution \- forwarded to LEWG

\#\#\#\# Papers that will be seen again by SG1

\* \[P3497R0\](https://wg21.link/P3497R0): Guarded Objects  
\* \[P3564R0\](https://wg21.link/P3564R0): Make the concurrent forward progress guarantee usable in \`bulk\`  
\* \[P3206R0\](https://wg21.link/P3206R0): A sender query for completion behaviour  
\* \[D3624R0\](https://wg21.link/D3624R0): get\_system\_scheduler (with concurrent forward progress\*)

\#\#\#\# SG1 Related Issues Seen

\* \[CWG2923\](https://wg21.link/CWG2923): A note in \\\[intro.progress\\\] that had been obsoleted by P2809 (Trivial infinite loops are not Undefined Behavior) was removed by unanimous consent.  
\* \[LWG4004\](https://wg21.link/LWG4004): SG1 agrees this is a defect and would like to see a paper addressing the issue.  
\* \[LWG4174\](https://wg21.link/LWG4174): SG1 agrees this is a defect and would like to see a paper addressing the issue.

\&nbsp;

\*\*\*\*\*

\#\#\# Networking Study Group (SG4) Progress

\*\*\*\*\*

SG4 met in Hagenberg to discuss “\[P3482R0\](https://wg21.link/P3482R0): Design for C++ networking based on IETF TAPS” \- a paper proposing a design for networking library based on senders/receivers. The paper shows a promising direction for secure-by-default networking in C++, and SG4 encouraged the author to continue work in P3842’s direction.

\&nbsp;

\*\*\*\*\*

\#\#\# Numerics Study Group (SG6) Progress

\*\*\*\*\*

The numerics group met for half a day, which was less than planned. We reviewed 5 papers.

\#\#\#\# Papers reviewed

\* \[P2746R7\](https://wg21.link/P2746R7): Deprecate and Replace Fenv Rounding Modes — We provided feedback to follow-up questions that came up.  
\* \[P3375R2\](https://wg21.link/P3375R2): Reproducible floating-point results — We would like to see more examples of problematic floating-point expressions.  
\* \[P3045R5\](https://wg21.link/P3045R5): Quantities and units library — Sadly we didn't have enough time to do the author/paper justice.  
\* \[P3495R0\](https://wg21.link/P3495R0): Remarks on Basic Statistics, P1708R9 — We agree with the need to document the design decisions that P3495R0 is asking about (publicly, not just in our internal minutes).  
\* \[P3565R0\](https://wg21.link/P3565R0): Virtual floating-point values — The paper was generally positively received but not forwarded to EWG yet because we would like more time to understand the consequences and allow time for alternative approaches to reach us. Keep an eye out on this paper if you're interested in improving our wording on floating-point.

\&nbsp;

\*\*\*\*\*

\#\#\# Compile-time Programming Study Group (SG7) Progress

\*\*\*\*\*

SG7 saw three papers proposing improvements to reflection targeting C++29:

\&nbsp;

\#\#\#\# Papers that were forwarded to EWG / LEWG

\* \[P3385R3\](https://wg21.link/P3385R3): Attributes Reflection — approved by SG7 and forwarded to EWG

\&nbsp;

\#\#\#\# Papers reviewed (require more work)  
\* \[P3420R1\](http://wg21.link/P3420R1): Reflection of Templates — this revision added functions for replacement and projection of names in templates.  
\* \[P3294R3\](http://wg21.link/P3294R3): Code Injection with Construct Sequences — was previously seen by EWG but brought back to SG7 for review of its updated design. Formerly called Token Sequences, these were rebranded to Construct Sequences to better convey how they can include reflections.

\&nbsp;

\*\*\*\*\*

\#\#\# Ranges Study Group (SG9) Progress

\*\*\*\*\*

SG9 met on Monday and Tuesday. 

\#\#\# Papers that were forwarded to LEWG

\* \[P3059R1\](https://wg21.link/P3059R1): Making user-defined constructors of view iterators/sentinels private — makes user-defined constructors of view iterators/sentinels private (we want it to be a DR for C++20\!). The fact that some of them were publicly accessible was most likely accidental.  
\* \[P3230R1\](https://wg21.link/P3230R1):  views::unchecked\_(take|drop) — adds \``views::unchecked_take` and `` views::unchecked_drop` ``. If you know that your range is big enough this can give you a 2x-3x speedup\!  
\* \[P3117R1\](https://wg21.link/P3117R1): Extending Conditionally Borrowed — extends conditionally borrowed for \``` views::transform` ``. That way, you can safely write code such as:  
\&nbsp;  
`` `return views::transform(this->my_container, [](auto elem) { return … });` ``

\&nbsp;

\#\#\#\# Papers reviewed (require more work)  
(we expect the following papers to be forwarded at the next meeting)

\* \[P3351R2\](https://wg21.link/P3351R2): views::scan — adds `views::scan` a lazy version of the `inclusive_scan` algorithm.  
\* \[P3411R1\](https://wg21.link/P3411R1): any\_view — adds a type-erased view adaptor. If you like ranges but don’t like templates, this allows you to define your range pipeline in these “.cpp” files we’ve been told about.  
\&nbsp;  
While discussing “\[P3555R0\](https://wg21.link/P3555R0): An infinite range concept”, which adds a concept to detect infinite ranges, we realized that infinite ranges don't even exist to begin with, even though the standard library has some of them.   
\&nbsp;  
Turns out that:  
\&nbsp;  
`` `views::iota(0) | views::take(10) ``, `for (auto x : views::iota(0)) { … break; }`\`  
\&nbsp;  
and arguably even:  
\&nbsp;  
`` `views::iota(0);` ``   
\&nbsp;  
are technically all undefined behavior\! \`(`` views::iota(0)` `` is an invalid range as the sentinel is not reachable in finitely many steps, and passing invalid ranges to standard library functions like \``` |` ``, \``` .begin()` ``, or \``` ~iota_view()` `` is undefined behavior.) We’re going to spend the next couple years or so tackling this tricky problem to make it well-defined.  
\&nbsp;  
\#\#\#\# Papers that did not get consensus

\*  \[P3329R0\](https://wg21.link/P3329R0):  Healing the C++ Filter View  
We also discussed and mostly rejected , which wants to solve some beginner pitfalls with `views::filter`. However, the design space is very constrained with regards to backwards compatibility and silent semantic changes of core concepts, so we encouraged more work by the author to come up with a separate view that solves these problems.  
\&nbsp;  
\*\*\*\*\*

\#\#\# Low Latency Study Group (SG14) Progress

\*\*\*\*\*

SG14 did not meet during the Hagenberg meeting. We continue to hold monthly telecons to discuss low latency, gaming, and embedded related papers.

\&nbsp;

\*\*\*\*\*

\#\#\# Tooling Study Group (SG15) Progress

\*\*\*\*\*

SG15 met for one session during Hagenberg to discuss how we plan to ship our deliverables now that we're not doing the Ecosystem IS. We decided to use the relatively new whitepaper process which has a significantly lower overhead than an IS, but some clarifications on the process are needed.

\#\#\#\# Papers reviewed

\* \[P1180R0\](https://wg21.link/P1180R0): Response to P1156 — We discussed the issues that header units can cause with build systems that use approximate scanning rather than precise scanning. The macros they bring in cause problems if they would impact other imports. CMake, MSVC, and Clang's scanner don't have this problem since they use precise scanning, so we're waiting for field experience from build systems that do approximate scanning to see what's actually needed here.

\&nbsp;  
\*\*\*\*\*

\#\#\# Text and Unicode Study Group (SG16) Progress

\*\*\*\*\*

SG16 did not meet in person during Hagenberg but continues to hold virtual meetings at its usual twice monthly cadence. As always, SG16 meeting summaries continue to be posted at \[SG16 GitHub\](https://github.com/sg16-unicode/sg16-meetings), though the SG16 chair has fallen behind in his duties, and so complete summaries will be posted in due time. 🙂

\&nbsp;

\*\*\*\*\*

\#\#\# Contracts Study Group (SG21) Progress (requires input from SG21 chair)

SG21 met for 1 day in Hagenberg.

\#\#\#\# Papers reviewed

\* \[P3583R0\](https://wg21.link/P3583R0): "Contracts, Types, & Functions" — an approach to make contracts work on function pointers. SG21 concluded that this approach doesn't quite work as proposed and the paper needs a revision; feedback to the author was given. This paper is now the \*third\* independent attempt to add contracts on function pointers, highlighting how hard this problem really is.  
\* \[P3400R0\](https://wg21.link/P3400R0): "Controlling Contract-Assertion Properties" — proposes to add labels to Contracts, which addresses many additional use cases that \[P2900\](https://wg21.link/P2900) on its own does not yet fully address. For example, you can have a label to specify in code that a particular contract assertion must always be enforced and can never be ignored or observed. This paper, too, needs a revision; feedback to the author was given.

\*\*\*\*\*

\#\#\# C / C++ Liaison Group (SG22) Progress

\*\*\*\*\*

SG22 did not meet in person during Hagenbert. We continue to run telecons by demand and provide feedback through the mailing list.

\&nbsp;

\*\*\*\*\*

\#\#\# Safety & Security Group (SG23) Progress

\*\*\*\*\*

SG23 met for a day in Hagenberg on Tuesday, with attendance affected by the discussions elsewhere on Contracts and Profiles

\&nbsp;

\#\#\#\# Papers forwarded to EWG/LEWG

\* \[P3566R0\](https://wg21.link/P3566R0): "You shall not pass char\* — Safety concerns working with unbounded null-terminated strings, forwarded to LEWG

\* \[P3442R1\](https://wg21.link/P3442R1): \[\[invalidate\_dereferencing\]\] attribute — , forwarded to EWG  
\* \[P3541R1\](https://wg21.link/P3541R1): Violation handlers vs noexcept — recommending that the issues described here are addressed before P3081 and P3100 are discussed further, forwarded to EWG

\#\#\#\# Papers reviewed

\* \[P3356R0\](https://wg21.link/P3356R0): non\_invalidating\_vector  
\* \[P3402R2\](https://wg21.link/P3402R2): A Safety Profile Verifying Class Initialization

\&nbsp;

\*\*\*\*\*

\# C++ Release Schedule

\*\*\*\*\*

\&nbsp;

\*\*\*NOTE: This is a plan not a promise. Treat it as speculative and tentative.\*\*\*

\*\*\*See \[P1000\](https://wg21.link/P1000), \[P0592\](https://wg21.link/P0592), \[P2000\](https://wg21.link/P2000) for the latest plan.\*\*\*

\&nbsp;

Meeting | Location | Objective  
\-|-|-  
\~\~2023 Summer Meeting\~\~ | \~\~Varna 🇧🇬\~\~ | \~\~First meeting of C++26.\~\~  
\~\~2023 Fall Meeting\~\~ | \~\~Kona 🇺🇸\~\~ | \~\~Design major C++26 features.\~\~  
\~\~2024 Winter Meeting\~\~ | \~\~Japan 🇯🇵\~\~ | \~\~Design major C++26 features.\~\~  
\~\~2024 Summer Meeting\~\~ | \~\~St. Louis 🇺🇸\~\~ | \~\~Design major C++26 features.\~\~  
\~\~2024 Fall Meeting\~\~ | \~\~Wrocław 🇵🇱\~\~ | \~\~C++26 major language feature freeze.\~\~  
\*\*2025 Winter Meeting\*\* | \*\*Hagenberg 🇦🇹\*\* | \*\*C++26 feature freeze. C++26 design is feature-complete.\*\*  
2025 Summer Meeting | Sofia 🇧🇬 | Complete C++26 CD wording. Start C++26 CD balloting ("beta testing").  
2025 Fall Meeting | Kona 🇺🇸 | C++26 CD ballot comment resolution ("bug fixes").  
2026 Winter Meeting | 🗺️ | C++26 CD ballot comment resolution ("bug fixes"), C++26 completed.  
2026 Summer Meeting | 🗺️ | First meeting of C++29.  
2026 Fall Meeting | 🗺️ | Design major C++29 features.  
2027 Winter Meeting | 🗺️ | Design major C++29 features.  
2027 Summer Meeting | 🗺️ | Design major C++29 features.  
2027 Fall Meeting | 🗺️ | C++29 major language feature freeze.

\&nbsp;

\*\*\*\*\*

\# Status of Major C++ Feature Development

\*\*\*\*\*

\&nbsp;

\*\*\*NOTE: This is a plan not a promise. Treat it as speculative and tentative.\*\*\*

\&nbsp;

\* IS \= International Standard. The C++ programming language. C++11, C++14, C++17, C++20, C+23, etc.

\* TS \= Technical Specification. "Feature branches" available on some but not all implementations. Coroutines TS v1, Modules TS v1, etc.

\* CD \= Committee Draft. A draft of an IS/TS that is sent out to national standards bodies for review and feedback ("beta testing").

\* WP \= Committee White Paper. Similar to TS, but is recommended by ISO for lightweight ISO process. For more information see \[SD-4\](https://isocpp.org/std/standing-documents/sd-4-wg21-practices-and-procedures)

\*\*Updates since the last Reddit trip report are in bold.\*\*

Feature | Status | Depends On | Current Target (Conservative Estimate) | Current Target (Optimistic Estimate)  
\-|-|-|-|-  
\[Senders\](https://wg21.link/P2300) | Plenary approved | | C++26 | C++26  
\[Networking\](https://wg21.link/P2171) | Require rebase on Senders | Senders | C++29 | C++29  
\[Linear Algebra\](https://wg21.link/P1673) | Plenary approved | | C++26 | C++26  
\[SIMD\](https://wg21.link/P1928) | Plenary approved | | C++26 | C++26  
\[Contracts\](https://wg21.link/P0542) | Forwarded to CWG, LWG | | C++26 | C++26  
\[Reflection\](https://wg21.link/P2996R0) | Forwarded to CWG, LWG | | C++26 | C++26  
\[Pattern Matching\](https://wg21.link/P1371) | EWG (discussed in Wroclaw) | | C++29 | C++29  
\[Profiles\](https://wg21.link/P3081), \[Syntax\](https://wg21.link/P3447) | EWG (discussed in Wroclaw) | Currently Targeting WP | WP | C++29  
\[Transactional Memory\](https://wg21.link/PXXXX) | SG5 approval | Currently Targeting WP | WP | WP 

\&nbsp;

\[\*\*Last Meeting's Reddit Trip Report.\*\*\](https://www.reddit.com/r/cpp/comments/1ienpc7/202411\_wroc%C5%82aw\_iso\_c\_committee\_trip\_report\_fifth/)

\&nbsp;

\*\*If you have any questions, ask them in this thread\!\*\*

\*\*Report issues by replying to the top-level stickied comment for issue reporting.\*\*

\&nbsp;  
\&nbsp;

\*/u/InbalL, Library Evolution (LEWG) Chair, Israeli National Body Chair\*

\*/u/jfbastien, Evolution (EWG) Chair\*

\*/u/erichkeane, Evolution Working Group Incubator (SG17, EWGI) Chair, Evolution (EWG) Vice Chair\*

\*/u/nliber, Library Evolution Incubator (SG18) Vice Chair, Library Evolution (LEWG) Vice Chair, Admin Chair, US National Body Vice Chair\*

\*/u/hanickadot, Compile-Time programming (SG7) Chair, Evolution (EWG) Vice Chair, Czech National Body Chair\*

\*/u/FabioFracassi, Library Evolution Vice Chair\*

\*/u/c0r3ntin, Library Evolution (LEWG) Vice Chair\*

\*/u/je4d, Networking (SG4) Chair, Reflection (SG7) Vice Chair\*

\*/u/V\_i\_r, Numerics (SG6) Chair\*

\*/u/foonathan, Ranges (SG9) Vice Chair\*

\*/u/bigcheesegs, Tooling (SG15) Chair\*

\*/u/tahonermann, Unicode (SG16) Chair\*

\*/u/mtaf07, Contracts (SG21) Chair\*

\*/u/timur\_audio, Contracts (SG21) Vice Chair\*

\*/u/eddie\_nolan\*

\*... and others ...\*  
