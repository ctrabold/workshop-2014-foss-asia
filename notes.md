# Links

Etsy have a great talk on how they do continuous deployment - http://channel9.msdn.com/Events/ALM-Summit/ALM-Summit-3/Continuous-Deployment-The-Dirty-Details - as well as one on how they do A/B testing and product development with hypothesis-driven development: http://www.infoq.com/presentations/Etsy-Deployment

There's currently a thread on the CD mailing list on how they do CD and code review: https://groups.google.com/forum/#!topic/continuousdelivery/9_5xpiHJZUc

---

Etsy:

We have built the culture in our Engineering team to assume everyone is going to do the right thing, and we should trust them. When that trust falls apart, I think of it as a bug in our hiring and on boarding processes.

---

Etsy

we think of committing to git as deploying to web servers (they happen nearly in sync). That doesn't mean that the code will be live to a public user. (Think: new class files, or new and unlinked JS or CSS, features that are gated off so that they are only available to staff members).

---

Check out the toolchain Facebook uses for kicks (it's intimidating): http://www.infoq.com/presentations/Facebook-Release-Process

Etsy have OSSed a lot of their toolchain on Github. Check out Deployinator for deployment: https://github.com/etsy/deployinator They also have some extensions for PHPUnit: https://github.com/etsy/phpunit-extensions If you're in to monitoring, there is some good stuff there. They also have a blog entry on static analysis for PHP: http://codeascraft.com/2012/08/10/static-analysis-for-php/ which has a link to a longer talk on the subject

For CI just use any CI system (you don't need your version control system to be built in PHP to use it with PHP -- same goes for your CI tool). Go will work fine, and as we know, it will soon be OSS :-) Etsy use Jenkins.

Migrations, again, you can just use dbdeploy.

Jez Humble, ThoughtWorks

---

Etsy

We find a lot of bugs through production monitoring that we would have never conceived of writing tests for.

Mike Brittain, Etsy

---

Etsy

Our Payments team, for example, is much more rigid about their review process than teams that, say, are running experiments at the UI level. It's not one-size-fits-all.

Mike Brittain, Etsy

Via https://groups.google.com/forum/m/#!forum/continuousdelivery


---

Gary’s story shows us that DevOps is not just for unicorns (e.g., Google, Amazon, Netflix, Etsy, Twitter, etc.) — DevOps is for any value stream where Development, Test and IT Operations must work together to achieve the organizational goals.

Via http://itrevolution.com/the-amazing-devops-transformation-of-the-hp-laserjet-firmware-team-gary-gruver/



http://java.dzone.com/articles/8-principles-continuous
http://www.thoughtworks.com/products/webinars/implementing-continuous-delivery
http://www.thoughtworks.com/products/webinars/understanding-mvp-connecting-continuous-delivery-lean-startup-movement
http://www.infoq.com/author/Jez-Humble
http://www.youtube.com/watch?v=TxydT76GbQA
