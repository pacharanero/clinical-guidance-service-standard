# Independent Health and Care (IHAC) UK Service Standard on the Production and Distribution of Clinical Guidance

DRAFT: February 2025

## About this service standard

1. In the absence of an official national service standard for the development, authoring, publication, and lifecycle management of Clinical Guidance, we propose this standard for all healthcare organisations and standard-setting bodies in the UK. We encourage collaborative improvement and eventual endorsement.

2. This service standard is designed to appeal to public, private, and third-sector healthcare organisations, and can be used internationally.

3. Comments and revisions are welcome and may be submitted as a GitHub Issue or preferably a GitHub Pull Request, including the proposed text and rationale.

## License ([CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/))

This service standard is released under a Creative Commons Attribution-NonCommercial 4.0 International License CC BY-NC 4.0. More details are available at [https://creativecommons.org/licenses/by-nc/4.0/](https://creativecommons.org/licenses/by-nc/4.0/).

Copyright of this work is owned by Independent Health and Care (IHAC) UK.

## Rationale for this service standard

1. **Rework is Wasting Our Time**: Experience of using and managing clinical guidance distribution systems indicates that there is considerable room for improvement in order to maximise the availability of the correct clinical guidance at the correct time, with minimal ‘clinical drag’. There is also a huge amount of duplication of effort across UK health and care creating localised or regionalised versions of clinical guidance when national guidance already exists.

2. **Poor Current User Experience**: The current clinical guidance distribution systems in use in UK healthcare vary widely in their fitness for purpose. Most are very poor. This has resulted in a range of clinical hazards including: difficulty in gaining access to guidance, outdated guidance remaining visible beyond review date, a confusing array of guidance sites, absent or unfit search facilities. Failure to instil innovation in clinical guidance authoring and distribution systems has also completely prevented the possibility of future development of ‘smart’ guidance.

3. **Too Many Organisations, Not Enough Agreement**: Clinical Guidance is produced and distributed by a very large range of organisations ranging in size and capability. It is unlikely that these myriad organisations would, of their own accord, create and agree to a service standard \- *especially if they are not currently equipped to achieve said service standard*. Therefore a community-driven, independent, open-source, user-needs-driven service standard has been created.

4. **A Better Way Is Possible**: Only by thinking smarter about how clinical guidance is authored and distributed can we realise some of the possibility of the future \- smarter and more reliable guidance, delivered using modern technical mechanisms directly to the point of care or educational need.

## Service Standard - Required Criteria

1. **Open Access**: Clinical Guidance **must** be publicly and openly available on the Internet without any kind of authentication step preventing read-only access. Open access simplifies and speeds access for end users.

2. **Link, Don’t Duplicate**: Regional Clinical Guidance **must** **not** be created where an acceptable National Clinical Guidance already exists. Provide a link to the existing National Clinical Guidance instead. Similarly, Local Clinical Guidance **must** **not** be created where an acceptable Regional or National Clinical Guidance already exists. Do not distribute a copy of the upstream guidance. **Provide a URL link to the *existing* Regional or National Clinical Guidance instead.**

3. **Open Publication Format**: Clinical Guidance **must** be published in a format that is natively visible in a web browser. Usually this means publishing the Clinical Guidance in HTML format. PDF and other formats which require the document to be downloaded and viewed in a separate, proprietary application (Adobe Reader, Microsoft Word) are **unacceptable**.

4. **Organisation Of Guidance**: Guidance **must** be listed in a way which allows sorting of the guidance in multiple ways, including but not limited to: ascending and descending alphabetical, ascending and descending date of publication.

5. **Searching of Guidance**: Clinical Guidance **must** be searchable with search tools fit for purpose. The search should extend to the document **content** as well as the title.

6. **Discoverability**: Guidance should be at a regular and conventional subdomain of the main organisation domain, such as guidance.organisation-name.org. This service standard does not as yet specify exactly what the subdomain should be, but it is likely that a convention, consisting of a few possible options for the subdomain will emerge from the adopters of this guidance.

7. **Authoring Format**: Clinical Guidance **must** be authored in a cross-platform compatible, non-proprietary data file format. No stipulation is made in this service standard regarding the specific file format used, but it is suggested to consider simple time-tested formats such as plain text and MarkDown as superior over time to more complex formats such as RTF, LaTeX or ODF. Authoring guidance in any kind of proprietary, database-backed Content Management System is expressly prohibited because of the difficulty of sharing, co-authoring, and future-proofing the work in such systems.

8. **Outdated Guidance Flagging**: Clinical Guidance which has passed its intended review date **must** be automatically highlighted as having become out of date by the clinical guideline distribution system.

9. **Preservation of Historic Guidance**: It is important that clinical guidance changes over time to reflect current best practice. In order that clinicians feel adequately defended in the case of medicolegal challenge, it **must** always be possible to show the exact state of clinical guidance as accessed at a particular point in time in the past. Modern open-source version control systems such as Git make this trivial to achieve.

## Service Standard - Desirable Criteria

1. **Preventative Outdated Guidance Flagging**: The guidance distribution platform **should** notify the original authors that guidance is nearing its intended review date, and remind regularly that review is due. Ideally this should prevent the situation in which

2. **Atomic URLs**: It **should** be possible to link to specific sections, paragraphs, or lines of the documentation via URL, not just a link to the whole document. It aids clinicians when they are able to refer colleagues via link directly to the part of the clinical guidance which is relevant to a specific case, informative in terms of training or education, or otherwise of specific interest. This requirement is simply, yet belatedly, bringing clinical guidance up to date with the power of the hyperlink, which has been a fundamental part of the ‘feature set’ of the Internet since its inception.

## Service Standard - Advanced Criteria

The following are criteria which will help us all move forward technologically in terms of the advanced usage of clinical guidance in the future.

1. **Clinical Terminology Tagging**: Clinical Guidance **should** be tagged with relevant entities from clinical terminology appropriate to the environment in which it is used. In UK General Practice this would be SNOMED-CT, for example. This Terminology Tagging would enable clinical systems to automatically guide the user towards the most appropriate Clinical Guidance based on the clinical terminology indicated by the electronic patient record..

2. **Standardised Metadata**: In order to enable better automated searching and discovery of Clinical Guidance, the metadata (data *about* the guidance, for example publication date, authors, review date) **should** be in a standardised, machine-readable, format. This allows for advanced automated features like: automatic flagging of post-review-date guidance, automatic linking of authors with declared conflicts of interest, automated author attribution and intelligent version control.

3. **Federation**: Clinical Guidance originating at *any* level in the healthcare system **should** be able to be federated both ‘upstream’ and ‘downstream’, with minimal additional rework. In ‘upstream’ federation, for example, a well-written, safe and comprehensive Local clinical guidance document should be able to be *offered* to be adapted for Regional or National level. Importantly, this *does not* **oblige** the upstream organisations to adopt the offered. **Downstream Federation**: In the ‘downstream’ federation model, it should be possible to take National level guidance and apply *templated* changes to it, to localise that guidance for maximum local applicability and usefulness *without completely rewriting it*. The advantage of this approach becomes most apparent the next time the upstream guidance is updated \- instead of triggering a series of urgent rewrites of downstream guidance, each downstream guidance body can each apply their templated changes to the new upstream guidance, check through, and publish.

## ‘Antipatterns’ (undesirable situations) and their solutions

* **Access Jeopardy Workarounds**: Users who are unsure that they will be able to access Clinical Guidance in a clinically reasonable time frame or without unnecessary authentication steps may tend to employ ‘workarounds’ \- such as downloading the guidance locally, creating a local repository of documents which will inevitably become out of date. This is a natural user response to the previous negative experiences of difficult access. **Solution**: Ensure that access is simple and fast, without authentication steps or other impediments.

* **Vanity Guidance Duplication**: Organisations may feel it necessary to endorse ‘upstream’ (Regional/National) guidance with a Local organisational logo or other non-functional change or embellishment. In order to do this, they create a new separate Local version of the guidance, resulting in duplication of effort, wasted resources, and later variation between the local and ‘upstream’ versions. This is a serious clinical risk and should be avoided. **Solution**: Do not vanity-brand perfectly valid upstream guidance. Instead consider requesting the addition of your organisational endorsement to the upstream version of the guidance.

* **Unauthorised Use Concerns**: Some Clinical Guidance documents include actionable forms which can be used for initiating referrals or other interventions across clinical services. A common organisational concern about making Clinical Guidance openly accessible is that ‘unauthorised’ individuals might then be able to use these referral forms. **Solution**: Do not use a log-in wall to prevent such abuse, this is known as ‘security by obscurity’ and always fails. Instead ensure that internal procedures are in place to verify that all forms have been completed by authorised persons. Ideally take steps to remove outdated mechanisms of actioning clinical requests, such as forms written in ‘digital paper’ (.docx, .pdf) and replace them with *modern, secure digital referral pathways* accessible only to suitably authorised individuals or their delegated administrative assistants..

## Authors and reviewers of this service standard

**Originating author**: Dr Marcus Baw, General Practitioner, UK.

**Reviewers**:
