# DynaTune
dynamic keyboard temperament for electronic music production


DynaTune
- dynamic keyboard temperament for chordal pitch-enhancement - 

keyboard players operate under a fundamental compromise
Every piano, organ, synthesizer, and digital keyboard relies on a static, two-dimensional tuning-system. Each note is fixed in advance. When you press a key, the pitch is predetermined. It does not bend. It does not negotiate. It does not adapt to the harmonic context around it.
That rigidity solves one problem — it allows modulation and consistent pitch across keys — but it creates another. Chords are never perfectly pure. Thirds stutter and sway off course. Fifths chortle and wobble menacingly. Fourths fidget and twitch nervously. Certain harmonies feel slightly tense even when they “should” feel resolved. These are not performance errors.  And equal temperament is not entirely to blame – the problem stems from an inherent limitation of all static, two-dimensional tunings.   
not all instruments are so constrained
Dynamic modulation of pitch remains the responsibility of musicianship on instruments which afford such possibility.  A violinist subtly adjusts pitch as they play. A guitarist bends notes. A singer reshapes intervals instinctively. These musicians can tune each note in real time to fit the harmony unfolding around them. They correct microtonal discrepancies on the fly. They lean into consonance.  
But for keyboards, unless you were one of the rare few who mastered alternate temperaments, retuned instruments manually, or performed on specially constructed microtonal keyboards, you were bound to a fixed grid. The instrument decided. You complied because you had no choice.
synthesis changed what is possible
Digital synthesis gives us the ability to retune pitches dynamically in real time. Instead of assigning one permanent frequency to each key, we can calculate pitch relationships based on harmonic context. When a chord is played, each note can be slightly adjusted to align with ideal interval ratios — producing harmonies that are mathematically cleaner and often more consonant.
Imagine pressing a C–E–G chord and having the E automatically settle into a perfectly pure 5:4 relationship above C. Imagine extended chords subtly reshaping themselves so their internal intervals align with ideal ratios rather than compromise approximations. The player does nothing differently. The instrument adapts.  This is what our approach explores.   
Chordal-root-referenced adjustments weighing less than a quartertone!
We start with what is reasonable: rational tunings.  The Scala tuning file collection has tens of thousands of such tunings readily available and DynaTune  will be Scala file literate in its coming implementations to make use of these.  Recognize that all equal temperaments have no reasonable place in our system other than to describe the legacy of inferior tuning regimes historic.  DynaTune  aims to become a viable and superior replacement for all equal temperaments.  
We anchor to a tonic-based framework and dynamically reconstruct each chord relative to its root – irrespective of the tuning and while preserving the character and flavor of that particular tuning.  Essentially the lowest note becomes the harmonic reference point and anchor.  Every other note in the chord is recalculated to match its ideal interval above that root. 
This results in the absence of accumulated drift, the absence of cascading distortion. DynaTune  achieves  contextual refinement while carefully preserving the flavor of any tuning.  DynaTune  boasts an aggregate deviation from the pitch reference of the intervals prior to adjustment typically less than a quartertone – half of a semitone or approximately 50 cents!  For the following tuning example the complete list of differences possible by all combinations of intervals for the specific tuning used in the example are 225/224, 126/125, 81/80, 64/63, 128/125, 36/35.  There is no coincidence in the fact that most of these are epimoric ratios, and pykna readily recognized by musicians and musicologists.   
An actual example
Using these note ratios from a just and nearly-palindromic tuning:

 0               1              2           3           4           5          6           7          8           9          10          11        12

1/1,      16/15,      10/9,      6/5,      5/4,      4/3,      7/5,      3/2,      8/5,      5/3,      9/5,      15/8,     2/1

  T            m2          M2         m3       M3       P4         tt          P5        m6       M6       m7         M7        O  


Where first row is scale degrees, second is the actual note ratios of the tuning, third is the abbreviated interval names such that T is tonic, miniscule m represents minor and majuscule M represents major and P denotes perfect tones and tt stands for tritone and O is for octave…

One observes that 3 semitones above the tonic {T) at the 3rd scale degree one finds the minor third (m3) with a note ratio value of 6/5.  Playing the tonic with scale degree 3 will always sound perfectly consonant.  Yet move the same interval up one set of keys and perfect consonance falls apart: playing the scale degrees 1 and 4 instead of 0 and 3 one does not hear a just and perfectly consonant minor third interval.  

We must take the note ratio of the 4th scale degree which is 5/4 and divide out of it the value of the 1st scale degree of 16/15 in order to obtain the actual interval between scale degrees 1 and 4.  We discover thereby why this chord sounds unhinged — the actual ratio played is 75/64 and shy of the magic proportion of 6/5 by a minor diesis of 128/125.  DynaTune  adjusts the note ratio of the 4th scale degree to compensate: augmenting 5/4 to 32/25 in order to attain a perfectly just minor third interval with chordal root in scale degree 1.

Johann Sebastien Bach’s dream
He struggled with the limitations of static keyboard-temperaments his whole life.  In recent times a student with the surname of Lehmann – a student at Juilliard School of music – discovered Bach had encoded his personal temperament into his signature.  Yet even with his works tuned to Lehmann’s discovered temperament fundamental limitations remain, as evident by the example above.  Static tunings and static temperaments remain stuck but a dynamic temperament like DynaTune  can finally bring perfect consonance home as synthesis and computation have changed what is possible for electronic music.  DynaTune  potentially achieves a slightly-modified version of Bach’s original dream: a well-tempered, ELECTRONIC clavier...
Microtonal pitch correction without exotic keyboards
It’s about giving keyboard players something they’ve historically envied: the ability to participate in microtonal pitch correction without needing decades of ear training or manual pitch control technique. The compromise of equal temperament is every note remains an imperfect, impure interval.  Yet despite this handicap the tuning regime of convention often sounded better than the alternatives, all of which were constrained to the limitations of static dimensionality.  
no Mozart required!
You don’t have to be an Amadeus to take advantage of DynaTune .  You don’t even have to have any skill or even know how to play any kind of instrument.  Heck, you don’t even have to know anything at all about music or even ever care.  You could even be tone-deaf or even just deaf.  We love and encourage your use of DynaTune  just the same, if not more.  DynaTune  lowers the access threshold in democratizing something that was once the domain of elite performers and a handful of master-level musicians who might exist in every generation of the world population.  Keyboard players can now meet the best guitar players eye to eye and rock just as hard, if not more.  And yet, a critical question remains.
is this even musically desirable?
Am I imagining this or does this really exist?  You decide.  Does dynamically purified harmony feel more consonant, more alive? Are there any rational tunings where DynaTune  falls apart?  I need you to break it, find where it sings and where it fails, and let’s fix it where it needs work.  I believe DynaTune  begins a revolution of music, rather than merely evolving musical tuning.  But perhaps I remain alone and perhaps you feel and hear it differently than do I.  Does it destabilize tonal expectations and destroy underlying, harmonic meanings? Will listeners experience it as clarity, or as unfamiliarity? In what context could it benefit a musical work?  Or perhaps no worth it has at all.  I don’t presume the answer for others.  I NEED YOUR HELP to determine this beyond myself.
an invitation
We are seeking collaboration — musicians, coders, composers, psychoacousticians, curious skeptics. We want to implement this system in practical electronic instruments and let artists decide. We want to test whether dynamically just reconstruction enhances musical expression or introduces new tradeoffs.
For too long, keyboard tuning has been a two-dimensional compromise grid. Digital instruments no longer need to remain confined there.  The question is not whether humanity can build adaptive harmonic engines.
We already have. 
The idea of a dynamic keyboard temperament which adjusts to the actual notes played is hardly new, either in theory or realization.  Predecessors and analogues exist, most notably Justonic and Hermode tuning. Yet they are not equivalent, remain biased to Western music and therefore not useful to non Western musical traditions, and assume just intonation scale without allowing for alternate tunings, such as Pythagorean, or thousands of other documented tunings in the Scala tuning file collection.  DynaTune  is universal in that it allows music traditions such as Arabic, Persian, Turkish, Indian and countless others to benefit from its pitch enhancement without losing the character and flavor of those traditions and their tunings.  Unlike its predecessors, DynaTune  makes no presumption of a 12 note octave.

We also do not limit adjustments to only the most consonant intervals in a scale.  Every note is modulated, taking harmonic correction further than any predecessors have dared to go.  We go farther, in every way.  Hermode and Justonic have locked their methodologies behind proprietary licenses and obfuscated patents.   
Ours is open source software
DynaTune  is open source, with a relatively accommodating license.  All specifications, code, derivations and implementations are restricted by its license to be open source and available for any and all to download and obtain in full and complete form.  It is free to use in non-commercial, and commercial music as long as a copy of its license are included with the piece of music.
Consider collaborating…
If you’re curious about reshaping harmony at the microtonal level — without abandoning the familiar keyboard — we invite you to explore, test, critique, and collaborate.
Let’s find out together whether this experiment reveals something we’ve only glimpsed in theory — a new flexibility for fixed-pitch instruments in the electronic age.  This particular approach may fail.  Yet the revolution must happen and outlive this, expand upon this..
Origin
DynaTune  derives from and remains part and parcel to the MANIFESTO AGAINST THE LIGHT, also known as CONTRALUX, and embodies the philosophy and heart of such.  As such It remains a gift to all of humanity, is open sourced, and seeks collaborators who might bring its realization into the production of music.  It originates — along with the MANIFESTO AGAINST THE LIGHT — with a Nobody Special by the name of Kiko - 
Frank O’Neill
1703 Mariachi Plaza de Los Angeles
Los Angeles, CA USA 90033

xorxecor@gmail.com
hexorxorxecor@gmail.com 


 
