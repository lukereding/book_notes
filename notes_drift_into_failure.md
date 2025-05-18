# drift into failure

Dekker

this book is about how complex systems fail not because of a breakdown in the components of a system, but because of breakdowns in relationships among components.

the author argues that our understanding of complex systems is heavily influenced by what he refers to as the 'legacy of newton and descartes', or what I would call more plainly reductionism: the idea that complex systems can be understood in terms of simple causes and effects, that understanding failure is just a matter of finding the broken component, and that there can be such a thing as 'root cause analysis' for failures of complex systems. the author discusses failure of systems in the context of what he calls 'drift into failure.' he details some reasons why systems drift into failure. the argues that complex systems slowly become less safe over time, often as a result of a series of locally rational decisions in response to constraints (time, money) that result in the system evolving to the limits of safe practice. he details several examples that show how drift towards failure is often clear in hindsight. he ends by arguing that the reductionist view of newton and descartes is an extremely blunt tool when trying to understand complex system failures, and that we need new mental models, tools, and vocabulary if we are to productively manage drift. ultimately, the author recommends that the language and models associated with systems theory and complexity theory are a useful step forward from reductionism, adn some more nebulous ideas about organization resilience, incorporation of a diversity of perspectives, and resilience engineering.

i think what the author written is true. i find much of the argument almost self-evident, but the implications of the argument for managing complex systems are actually quite strong.

the implications of the argue are actually quite broad even if they don't appear to be on first glance. the implication of moving away from reductionism and towards an embrace of systems thinking means that understanding how accidents happen is no longer a matter of 'root cause analysis'—such an analysis is predicated on a foundation of reductionism and is incompatible with a systems view of accidents. this observation clearly also has implications for understanding accountability when dealing with complex systems. this realization also implies that retroactive analysis of causes of past failures are extremely limited in their usefulness, as it is unlikely in complex systems for the same accident to happen the same way multiple times. and this realization also emphasizes the need for diversity in thought and perspectives, especially in complex system where no one can understand or conceptualize the system as a whole.

in practice, some practices that embrace these realizations:

- asking "What workaround did you adopt last month that would’ve seemed unacceptable six months ago?" This helps highlight if and where safety margins are being eroded
- compile all the safety buffers in practice in one place, ideally with quantitative metrics that can be tracked over time
- using practices like STAMP instead of RCA
- "stop the line" authority
- blameless incident reporting


Other notes I took:

- reasons for drift
  - scarcity / competition
  - decrementalism
  - sensitivity to initial conditions
  - unruly technology
  - contribution of the protective structure
- locally rational decisions != globally rational decisions
- accidents in complex systems come from a breakdown of relationships, not necessarily a breakdown of parts
- in complex systems, the liklihood that an accident happens the same way twice is very low. therefore, retroactive analysis is limited in its usefulness. _there is a difference between explaining way a particular event happened and understanding where attention should be focused to ensure tat similar accidents don't happen in the future_
- in complex systems, introducing new components or redundencies to reduce errors often results in _more_ errors, because it results in a ballooning in the number of relationships and makes the system more difficult to reason about
- 'blame the component' view of failure is an outgrowth of reductionism
- drift always deals with a change in norms or what is considered acceptable
- being the insider of a complex system—like an expert of some component of the system—can make systems thinking impossible



MRM implications:
"being the insider of a complex system—like an expert of some component of the system—can make systems thinking impossible"